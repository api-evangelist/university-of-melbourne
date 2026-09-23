# examples/

Every file here is a **verbatim capture of a live response on 2026-08-19**, not a hand-written
sample. Each one is listed with the exact request that produced it.

| File | Request | Operator |
|---|---|---|
| `university-of-melbourne-sudo-datasets-example.json` | `GET https://sudo.eresearch.unimelb.edu.au/api/v2/datasets?page_size=1` → 200 | institution |
| `university-of-melbourne-minerva-access-root-example.json` | `GET https://minerva-access.unimelb.edu.au/server/api` → 200 `application/hal+json` | institution |
| `university-of-melbourne-minerva-access-communities-example.json` | `GET https://minerva-access.unimelb.edu.au/server/api/core/communities?size=2` → 200 | institution |
| `university-of-melbourne-oai-pmh-identify-example.xml` | `GET .../server/oai/request?verb=Identify` → 200 `text/xml` | institution |
| `university-of-melbourne-oai-pmh-listmetadataformats-example.xml` | `GET .../server/oai/request?verb=ListMetadataFormats` → 200 `text/xml` | institution |
| `university-of-melbourne-idp-saml-metadata-example.xml` | `GET https://idp.unimelb.edu.au/idp/shibboleth` → 200 `application/xml` | institution |
| `university-of-melbourne-sso-openid-configuration-example.json` | `GET https://sso.unimelb.edu.au/.well-known/openid-configuration` → 200 | **tenant** (Okta) |
| `university-of-melbourne-arcgis-hub-ogc-records-example.json` | `GET https://spatialdata-uom.opendata.arcgis.com/api/search/v1` → 200 | **tenant** (Esri ArcGIS Hub) |

provenance:
  generated: 2026-08-19
  method: probed
  source: direct HTTPS requests, browser User-Agent, statuses recorded above
