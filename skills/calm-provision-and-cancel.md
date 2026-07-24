---
name: Provision and cancel a Calm subscription for a partner user
description: >-
  Authenticate a partner service against the Calm Partner API, link a partner user
  to a Calm subscription (returning the login/signup redirect), and later cancel
  that subscription to prevent auto-renewal.
api: openapi/calm-partner-api-openapi.yml
operations:
- authorize
- linkUser
- cancelUser
---

# Provision and cancel a Calm subscription

Use the Calm Partner API to onboard a member of your organization onto Calm Business /
Calm Health and to off-board them. Base URL: `https://auth.calm.com` (production) or
`https://auth-ga.aws-dev.useast1.calm.com` (development).

## 1. Authenticate (`authorize`)

`POST /v0/authorize` with a JSON body:

- `client_id`, `client_secret` — issued by Calm partner onboarding (per environment)
- `grant_type`: `client_credentials`
- `scope`: `b2b.users.integrate,b2b.subscription.cancel`

Response carries `access_token` (a Bearer JWT), `token_type`, `expires_at`, `token_id`.
Cache the token until `expires_at`; re-authenticate on `403` (invalid authorization/scope).

## 2. Link a partner user (`linkUser`)

`POST /v0/b2b/users/link` with `Authorization: Bearer {access_token}` and body:

- `partner_user_id` — a stable partner-generated GUID for the user (required)
- `error_url` — optional custom error-page redirect

By default the call returns a `303` redirect whose `Location` carries a `calm-link-token`;
send the user there to log in or create a Calm account. For a programmatic/agent flow add
`?pseudo_redirect=1` to get a `200` JSON body with `redirect_location` instead. Handle `400`
(invalid request) and `401` (token expired — re-run step 1).

## 3. Cancel a subscription (`cancelUser`)

`DELETE /v0/b2b/users/{partner_user_id}` with the Bearer token. This prevents auto-renewal.
The response returns `status` = `canceled` (with `calm_user_id` and `expires`) or `not_found`.
The operation is semantically idempotent: repeating it on an already-cancelled or unknown user
returns `not_found` rather than erroring.

## Notes

- Errors are bare HTTP status codes (no problem+json envelope) — see `errors/calm-problem-types.yml`.
- No idempotency-key header is published; see `conventions/calm-conventions.yml`.
- Bulk eligibility is also supported out-of-band via SFTP CSV uploads and SAML 2.0 SSO
  (`partner.calm.com/docs/sso`).
