# University of Melbourne (university-of-melbourne)

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

The University of Melbourne is Australia's leading research university, a Group of Eight member
founded in 1853. Re-profiled on **2026-08-19** under the API Evangelist **university pipeline**,
which settles **who operates each surface** before saving anything — because at a university almost
every apparent API is a vendor contract running under the institution's name.

- APIs.json: https://raw.githubusercontent.com/api-evangelist/university-of-melbourne/refs/heads/main/apis.yml

## Type

`x-type: university` / `x-category: Public Research University` / Provider / Public

## Tags

University, Higher Education, Education, Australia, Group of Eight, Research, Research Data,
Research Repository, Open Data, Geospatial, Identity Federation, Library

## Surfaces, by operator

Every entry in `apis.yml` carries an `x-operator`. Four are the institution's own; four are
tenancies on someone else's platform, recorded as relationships with **no vendor contract saved
under this slug**.

### `x-operator: institution` — the University runs these

| Surface | Base URL | Verified 2026-08-19 |
|---|---|---|
| **Spatial Urban Data Observatory (SUDO)** — GeoNode, 7,417 spatial datasets, unauthenticated | `https://sudo.eresearch.unimelb.edu.au/api/v2` | 200, `total: 7417` |
| **Minerva Access REST API** — self-hosted DSpace 7.6, 223 communities | `https://minerva-access.unimelb.edu.au/server/api` | 200 `application/hal+json` |
| **Minerva Access OAI-PMH 2.0** — 14 metadata formats, two locally built | `https://minerva-access.unimelb.edu.au/server/oai/request` | 200 `text/xml` |
| **Shibboleth Identity Provider** — SAML 2.0 metadata, registered in AAF/eduGAIN | `https://idp.unimelb.edu.au/idp/shibboleth` | 200 `application/xml` |

### `x-operator: tenant` — the University's data, someone else's contract

| Surface | Platform | Evidence |
|---|---|---|
| **Melbourne Data** `melbourne.figshare.com` | Figshare (Digital Science) | DataCite client `UNIMELB.REPO1` |
| **Open Spatial Data Portal** `spatialdata-uom.opendata.arcgis.com` | Esri ArcGIS Hub | DCAT-US 1.1 feed + OGC API Records, both 200 |
| **University SSO** `sso.unimelb.edu.au` | Okta Identity Cloud | OIDC discovery + RFC 8414 metadata, both 200 |
| **Internal API programme** | Boomi | Vendor case study only — no institutional URL exists |

## What is actually notable here

1. **SUDO is real, and nobody has catalogued it.** An open, unauthenticated JSON API over 7,417
   spatial datasets, run by the University on its own host. It is also **broken in two ways** we
   record rather than smooth over: the TLS certificate is issued for
   `staging.unimelb-sudo.cloud.edu.au` and matches no other name, so a conformant client cannot
   connect; and `/api/v2/categories` times out at 60s while sibling collections answer normally.
2. **The OAI-PMH endpoint proves institutional engineering.** Of fourteen metadata formats, two are
   the University's own — `umbl` (University of Melbourne Library) and a `trove` crosswalk into the
   National Library of Australia under a `uom` namespace path. Neither ships with stock DSpace.
   That is the difference between running a package and operating a surface.
3. **The identity federation is the find most university profiles miss.** A self-hosted Shibboleth
   IdP with public SAML 2.0 metadata, registered in the Australian Access Federation alongside ten
   other `unimelb.edu.au` entities. Institution-operated by definition, machine-readable, and
   almost never listed anywhere.
4. **No Figshare contract is stored here.** `api.figshare.com/v2` was attributed to 25 institutions
   in the June 2026 cohort. Melbourne's Figshare relationship is recorded as a tenancy and the
   vendor's specification stays in the vendor's repository.

## What the University does not publish

No OpenAPI or any machine-readable contract for anything it runs (GeoNode's own `/api/v2/openapi`
returns 404 on this deployment). No developer portal — `api.`, `developer.` and `data.unimelb.edu.au`
do not resolve. No changelog, no status page, no rate-limit signal, no support channel for any
surface. No public course-catalog or timetable API. Three surfaces use three different error
conventions and none is RFC 9457; OAI-PMH reports failure with HTTP 200, which is
specification-correct and worth knowing before you write a harvester.

**The three OpenAPI documents in `openapi/` are ours**, marked `method: derived`, built only from
endpoints that returned 200 on 2026-08-19. They must never be read as contracts the University
publishes.

## Artifacts

| Directory | What is in it | Method |
|---|---|---|
| `openapi/` + `openapi/_original/` | 3 derived contracts (SUDO, DSpace REST, OAI-PMH) | derived |
| `json-schema/` | SUDO dataset, Minerva Access community | derived |
| `examples/` | 8 verbatim live captures, each with its request and status | probed |
| `conformance/` | `education` regime standards: **oai-pmh, shibboleth, saml** confirmed institution-side, **datacite** confirmed tenant-side | probed |
| `authentication/` | per-surface auth posture, split by operator | probed |
| `scopes/` | the Okta OIDC scope set — marked `x-operator: tenant` | probed |
| `errors/` | three error conventions + the TLS and timeout defects + a soft-404 | probed |
| `vocabulary/` | the 14 OAI-PMH metadata formats, local ones called out | probed |
| `rules/` | 10 governance rules with the observed result for each | derived |
| `lifecycle/` | version signals + ~60 unprobed DSpace link relations, listed not invented | probed |
| `json-ld/` | organization record with ROR `01ej9dk98`, GRID, ISNI, Wikidata, Handle prefix 11343 | searched |

## Coverage

`x-coverage.state: covered`. Real probes ran and found real institution-operated surfaces. What is
thin here is documentation, not surface. Two probe limitations are declared in `apis.yml`: the whole
`*.unimelb.edu.au` marketing and student web estate sits behind Cloudflare bot management and
returned HTTP 403 to every client tried (recorded as live-but-unreadable, never dead), and SUDO
could only be reached with certificate verification disabled.

## Timestamps

- Created: 2026-06-03
- Modified: 2026-08-19

## Maintainers

- Kin Lane — kin@apievangelist.com
