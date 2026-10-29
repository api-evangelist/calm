# Calm

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

Calm is a leading consumer mental-wellness company whose app offers guided meditations, Sleep Stories, breathing programs, mindfulness masterclasses, and soundscapes. Beyond the direct-to-consumer app, Calm sells two B2B products: Calm Business, which delivers the Calm experience to employers as an employee wellness benefit, and Calm Health, a clinical mental-health offering for health plans and large self-insured employers. Both are powered by the Calm Partner API, an OAuth 2.0 client-credentials REST surface that partner HR and benefits systems use to provision, link, and cancel Calm subscriptions for their members, alongside SAML 2.0 IdP-initiated SSO and SFTP eligibility-file uploads. Calm is a portfolio company of Lightspeed Venture Partners.

**Areas:** Company · Mental Health · Wellness · Meditation · Mindfulness · Sleep · Employee Benefits · Health · B2B · Subscription

## Calm on APIs.io

Everything profiled for Calm is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/calm/](https://apis.io/providers/calm/)** — or go straight to one of the APIs or properties below.

### APIs (2)

- [Calm Authentication API](https://apis.io/apis/calm/calm-authentication-api/) — Obtain a JWT access token via OAuth 2.0 client credentials.
- [Calm Subscriptions API](https://apis.io/apis/calm/calm-subscriptions-api/) — Link and cancel partner-user Calm subscriptions.

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### MCP servers (1)

Model Context Protocol servers that expose the API to agents.

- [calm-partner](https://apis.io/servers/calm/calm-partner/)

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Calm Agentic Access](https://apis.io/agentic-access/calm/calm-agentic-access/)

#### JSON Schema (2)

The data models the API reads and writes.

- [Calm Eligibility File Row](https://apis.io/schemas/calm/calm-eligibility-file/)
- [Calm Partner User](https://apis.io/schemas/calm/calm-partner-user/)

#### JSON-LD (1)

Linked-data contexts for the provider's vocabulary.

- [Calm Context](https://apis.io/jsonld/calm/calm-context/)

#### Vocabulary (1)

The provider's domain terms, defined.

- [Calm Vocabulary](https://apis.io/vocabularies/calm/calm-vocabulary/)

#### Examples (3)

Example requests and responses.

- [Calm Authorize Example](https://apis.io/examples/calm/calm-authorize-example/)
- [Calm Cancel User Example](https://apis.io/examples/calm/calm-cancel-user-example/)
- [Calm Link User Example](https://apis.io/examples/calm/calm-link-user-example/)

#### Collections (3)

Postman and Open Collection request collections.

- [Calm Partner Authentication API](https://apis.io/collections/calm/open-calm-authentication-api/)
- [Calm Partner API](https://apis.io/collections/calm/open-calm-partner-api/)
- [Calm Partner Authentication Subscriptions API](https://apis.io/collections/calm/open-calm-subscriptions-api/)

#### Overlays (1)

OpenAPI overlays, including conversational phrasing for each operation.

- [Calm Partner Api Overlay](https://apis.io/overlays/calm/calm-partner-api-overlay/)

#### Governance rules (1)

Spectral rulesets for the provider's contracts.

- [Calm — jsonschema rules](https://apis.io/rules/calm/calm-jsonschema-spectral-rules/)

#### Security (2)

Authentication, trust centre, and vulnerability disclosure.

- [Calm Authentication](https://apis.io/security/calm/calm-authentication/)
- [Calm Domain Security](https://apis.io/security/calm/calm-domain-security/)

#### OAuth scopes (1)

The permissions the API asks for.

- [Calm Scopes](https://apis.io/scopes/calm/calm-scopes/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://www.calm.com)
- [Documentation](https://partner.calm.com/docs/api)
- [Getting started](https://partner.calm.com/docs/api)
- [API reference](https://partner.calm.com/docs/api)
- [Pricing](https://business.calm.com/)
- [Support](https://support.calm.com/hc/en-us)
- [Blog](https://blog.calm.com)
- [Trust centre](https://health.calm.com/trust)
- [Terms of service](https://www.calm.com/terms)
- [Privacy policy](https://www.calm.com/privacy)
- [GitHub](https://github.com/calm)
- [Status](https://status.calm.com)

## API Evangelist rating

**Kin Score 50.1** — developing · rubric 0.25.0 · scored 2026-10-23

| Facet | Score |
|---|---|
| Discoverability | 74.1 |
| Contract quality | 56.0 |
| Contract governance | 14.4 |
| Operational transparency | 18.4 |
| Developer ergonomics | 66.1 |
| Access clarity | 44.7 |

**Agent readiness 25.1** — agent-aware

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | derived (partial credit) |
| Reversibility Documented | documented (partial credit) |
| MCP Server | — |
| Auth Clarity | negotiable (partial credit) |
| Idempotency | — |
| Error Semantics | derived (partial credit) |
| OpenAPI Examples | — |
| Rate Limit Signal | — |
| Event Surface Described | — |
| Agent Skills | derived (partial credit) |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |
| Pagination Ratio | na |
| Operation Distinctiveness | distinct |

**Regulatory alignment 32.8** — Health

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/calm/](https://apis.io/providers/calm/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Calm: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/calm/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
