# University of Melbourne (university-of-melbourne)

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
