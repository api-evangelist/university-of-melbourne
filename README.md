# University of Melbourne

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

The University of Melbourne is Australia's leading research university, a Group of Eight member founded in 1853 and ranked in the world top 25. Its programmable footprint is small, unmarketed and genuinely its own in two places — which is more than most of this cohort can say. The institution operates a public, unauthenticated JSON API over 7,417 spatial datasets in the Spatial Urban Data Observatory (GeoNode, on unimelb.edu.au), and it runs Minerva Access — a self-hosted DSpace 7.6 repository on its own ITS infrastructure — exposing both a HAL+JSON REST API and an OAI-PMH 2.0 harvesting endpoint whose fourteen metadata formats include two the Library built itself (`umbl`, and a `trove` crosswalk for the National Library of Australia). It also operates its own Shibboleth SAML 2.0 identity provider, registered in the Australian Access Federation and reachable as public metadata. None of these is documented as a product: there is no developer portal, no OpenAPI, no changelog, no status page, no rate-limit signal and no support channel for any of them, and the University publishes no machine-readable contract for anything it runs. Everything else that looks like a University of Melbourne API is a tenancy — Melbourne Data on Figshare, the open spatial portal on Esri ArcGIS Hub, web SSO on Okta, the internal API programme on Boomi. Those relationships are recorded here with `x-operator: tenant` and no vendor contract is stored under this slug.

**Areas:** University · Higher Education · Education · Australia · Group of Eight · Research · Research Data · Research Repository · Open Data · Geospatial · Identity Federation · Library

## University of Melbourne on APIs.io

Everything profiled for University of Melbourne is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/university-of-melbourne/](https://apis.io/providers/university-of-melbourne/)** — or go straight to one of the APIs or properties below.

### APIs (9)

- [Shibboleth Identity Provider — SAML 2.0 Metadata](https://apis.io/apis/university-of-melbourne/shibboleth-identity-provider/) — The University's own Shibboleth identity provider, entityID https://idp.unimelb.edu.au/idp/shibboleth, serving public SAML 2.0 metadata at that URL…
- [Melbourne Data — Research Data Repository (Figshare tenancy)](https://apis.io/apis/university-of-melbourne/melbourne-data-figshare/) — TENANT RELATIONSHIP, recorded deliberately and with no contract saved. melbourne.figshare.com is the University of Melbourne's research data repository,…
- [Open Spatial Data Portal (Esri ArcGIS Hub tenancy)](https://apis.io/apis/university-of-melbourne/spatial-open-data-arcgis-hub/) — TENANT RELATIONSHIP. An Esri ArcGIS Hub site publishing University of Melbourne campus GIS layers — building, road and tree-canopy footprints. Verified live…
- [University SSO — OpenID Connect Discovery (Okta tenancy)](https://apis.io/apis/university-of-melbourne/sso-okta/) — TENANT RELATIONSHIP. sso.unimelb.edu.au is an Okta Identity Cloud tenancy running under a University vanity hostname. The OpenID Connect discovery document…
- [Internal API Management Programme (Boomi tenancy) — Gated](https://apis.io/apis/university-of-melbourne/boomi-internal-api-portal/) — TENANT RELATIONSHIP, and a weak one. The University of Melbourne runs a Boomi-based internal API management programme and developer portal for staff and…
- [University of Melbourne Core API](https://apis.io/apis/university-of-melbourne/university-of-melbourne-core-api/) — Repository content hierarchy
- [University of Melbourne Datasets API](https://apis.io/apis/university-of-melbourne/university-of-melbourne-datasets-api/) — Spatial datasets held in the observatory
- [University of Melbourne Discovery API](https://apis.io/apis/university-of-melbourne/university-of-melbourne-discovery-api/) — HAL root document
- [University of Melbourne OAI PMH API](https://apis.io/apis/university-of-melbourne/university-of-melbourne-oai-pmh-api/) — Open Archives Initiative Protocol for Metadata Harvesting 2.0

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### MCP servers (1)

Model Context Protocol servers that expose the API to agents.

- [Moved to /providers/university-of-melbourne/](https://apis.io/servers/university-of-melbourne/university-of-melbourne/)

#### JSON Schema (2)

The data models the API reads and writes.

- [Minerva Access Community](https://apis.io/schemas/university-of-melbourne/university-of-melbourne-minerva-access-community/)
- [SUDO Dataset](https://apis.io/schemas/university-of-melbourne/university-of-melbourne-sudo-dataset/)

#### JSON-LD (2)

Linked-data contexts for the provider's vocabulary.

- [University Of Melbourne Context](https://apis.io/jsonld/university-of-melbourne/university-of-melbourne-context/)
- [University Of Melbourne Organization Context](https://apis.io/jsonld/university-of-melbourne/university-of-melbourne-organization/)

#### Examples (5)

Example requests and responses.

- [University Of Melbourne Arcgis Hub Ogc Records Example](https://apis.io/examples/university-of-melbourne/university-of-melbourne-arcgis-hub-ogc-records-example/)
- [University Of Melbourne Minerva Access Communities Example](https://apis.io/examples/university-of-melbourne/university-of-melbourne-minerva-access-communities-example/)
- [University Of Melbourne Minerva Access Root Example](https://apis.io/examples/university-of-melbourne/university-of-melbourne-minerva-access-root-example/)
- [University Of Melbourne Sso Openid Configuration Example](https://apis.io/examples/university-of-melbourne/university-of-melbourne-sso-openid-configuration-example/)
- [University Of Melbourne Sudo Datasets Example](https://apis.io/examples/university-of-melbourne/university-of-melbourne-sudo-datasets-example/)

#### Governance rules (1)

Spectral rulesets for the provider's contracts.

- [University of Melbourne API Rules](https://apis.io/rules/university-of-melbourne/university-of-melbourne-rules/)

#### Security (3)

Authentication, trust centre, and vulnerability disclosure.

- [University Of Melbourne Authentication](https://apis.io/security/university-of-melbourne/university-of-melbourne-authentication/)
- [University Of Melbourne Domain Security](https://apis.io/security/university-of-melbourne/university-of-melbourne-domain-security/)
- [University Of Melbourne Vulnerability Disclosure](https://apis.io/security/university-of-melbourne/university-of-melbourne-vulnerability-disclosure/)

#### OAuth scopes (1)

The permissions the API asks for.

- [University Of Melbourne Scopes](https://apis.io/scopes/university-of-melbourne/university-of-melbourne-scopes/)

#### Plans and pricing (1)

Published plans, tiers and prices.

- [University Of Melbourne Plans Pricing](https://apis.io/plans/university-of-melbourne/university-of-melbourne-plans-pricing/)

#### Rate limits (1)

Published request limits.

- [University Of Melbourne Rate Limits](https://apis.io/rate-limits/university-of-melbourne/university-of-melbourne-rate-limits/)

#### FinOps (1)

What the API costs to run, by operation.

- [University Of Melbourne Finops](https://apis.io/finops/university-of-melbourne/university-of-melbourne-finops/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://www.unimelb.edu.au/)
- [Terms of service](https://policy.unimelb.edu.au/)
- [Privacy policy](https://about.unimelb.edu.au/strategy/governance/compliance-obligations/privacy)

## API Evangelist rating

**Kin Score 29.6** — thin · rubric 0.25.0 · scored 2026-10-23

| Facet | Score |
|---|---|
| Discoverability | 65.0 |
| Contract quality | 26.7 |
| Contract governance | 33.3 |
| Operational transparency | 21.1 |
| Developer ergonomics | 19.0 |
| Access clarity | 15.8 |

**Agent readiness 36.1** — agent-ready

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | — |
| Reversibility Documented | na |
| MCP Server | verified |
| Auth Clarity | bearer (partial credit) |
| Idempotency | na |
| Error Semantics | — |
| OpenAPI Examples | verified |
| Rate Limit Signal | derived (partial credit) |
| Event Surface Described | — |
| Agent Skills | — |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | na |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |
| Pagination Ratio | na |
| Operation Distinctiveness | distinct |

**Regulatory alignment 36.3** — Education & Research

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/university-of-melbourne/](https://apis.io/providers/university-of-melbourne/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for University of Melbourne: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/university-of-melbourne/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
