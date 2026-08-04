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
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

The University of Melbourne is Australia's leading research university, ranked #24 in the QS World University Rankings 2025. Its public developer and API footprint is modest and federated: the Library runs the Minerva Access institutional repository (DSpace 7.6) with public OAI-PMH and REST APIs, and the institution publishes campus GIS data through an ArcGIS Hub open spatial-data portal. An internal Boomi-based API management developer portal exists for staff and students but is gated and not publicly documented.

- APIs.json: https://raw.githubusercontent.com/api-evangelist/university-of-melbourne/refs/heads/main/apis.yml
- Run with Naftiko: https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=university-of-melbourne-api-evangelist&utm_content=repo

## Type

Index / Consumer / 3rd-Party

## Tags

Education, Higher Education, University, Australia, Open Data, Research, Library, Repository

## APIs

- **Minerva Access OAI-PMH** — Public OAI-PMH 2.0 metadata-harvesting interface for the University Library Digital Repository (DSpace 7.6). Docs: https://minerva-access.unimelb.edu.au/ — base URL `https://minerva-access.unimelb.edu.au/server/oai/request`
- **Minerva Access DSpace REST API** — DSpace 7.6 REST/HAL API exposing communities, collections, items and bitstreams. Docs: https://minerva-access.unimelb.edu.au/ — base URL `https://minerva-access.unimelb.edu.au/server/api`
- **Open Spatial Data Portal (ArcGIS Hub)** — Campus GIS layers (buildings, roads, tree canopy) via standard ArcGIS Hub query/download APIs. Docs: https://spatialdata-uom.opendata.arcgis.com/
- **Internal API Management Developer Portal (Boomi) — Gated** — Self-service internal data APIs for staff/students; gated behind university authentication, not publicly documented. Reference: https://boomi.com/blog/university-of-melbourne-innovates-with-api-driven-strategy/

## Plans

- plans/university-of-melbourne-plans-pricing.yml

## Rate Limits

- rate-limits/university-of-melbourne-rate-limits.yml

## FinOps

- finops/university-of-melbourne-finops.yml

## Timestamps

- Created: 2026-06-03
- Modified: 2026-06-03

## Common Properties

- Website: https://www.unimelb.edu.au/
- GitHub: https://github.com/unimelb
- LinkedIn: https://au.linkedin.com/school/university-of-melbourne/
- Authentication (SSO): https://sso.unimelb.edu.au/

## Notes

All endpoints listed were verified live where possible. The Minerva Access OAI-PMH and DSpace REST roots and the ArcGIS Hub spatial portal returned HTTP 200 on 2026-06-03. The official website (https://www.unimelb.edu.au/) returns 403 to automated clients due to bot protection but serves normally in a browser. The Boomi developer portal is referenced from a public vendor case study but is gated; no public endpoints were confirmed and none were invented. Central SSO uses Okta with OAuth 2.0 / OpenID Connect but exposes no public API program. See review.yml for the full probe log.

## Maintainers

- Kin Lane — kin@apievangelist.com
