# NOAA — National Oceanic and Atmospheric Administration (noaa-gov)

The National Oceanic and Atmospheric Administration (NOAA) is the United States scientific and regulatory agency within the Department of Commerce charged with monitoring oceanic and atmospheric conditions, charting the seas, conducting deep-sea exploration, managing fishing and protection of marine mammals, and providing weather, climate, space weather, and ecosystem forecasts and warnings. NOAA's developer surface spans six line offices — the National Weather Service (NWS), the National Environmental Satellite, Data, and Information Service (NESDIS) including the National Centers for Environmental Information (NCEI), the National Ocean Service (NOS) including Tides & Currents (CO-OPS), the National Marine Fisheries Service (NMFS / NOAA Fisheries), the Office of Oceanic and Atmospheric Research (OAR), and the Office of Marine and Aviation Operations (OMAO). NOAA exposes free, open APIs at api.weather.gov, services.swpc.noaa.gov, api.tidesandcurrents.noaa.gov, ncei.noaa.gov/access, ERDDAP servers across line offices, the National Data Buoy Center (NDBC), and bulk forecast model output (GFS, GEFS, HRRR, GOES) through the NOAA Open Data Dissemination (NODD) program on AWS, GCP, and Azure.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/noaa-gov/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/noaa-gov/refs/heads/main/apis.yml)

## Tags

- Weather
- Climate
- Ocean
- Space Weather
- Government
- Open Data
- Forecast
- Marine
- Atmospheric
- Hydrology
- Satellite
- Fisheries
- Aviation
- Emergency Management

## Timestamps

- **Created:** 2026-05-25
- **Modified:** 2026-05-25

## APIs

### National Weather Service API (api.weather.gov)

The National Weather Service public REST API delivers real-time weather forecasts, alerts, observations, gridded forecast data, aviation weather products, and metadata for offices, zones, and radar stations across the United States and US territories. Responses default to GeoJSON with content negotiation for JSON-LD, CAP, ATOM, and DWML. No API key is required — only a unique User-Agent string identifying the calling application. Stable production endpoint at api.weather.gov, current spec version 3.9.2.

- **Human URL:** [https://www.weather.gov/documentation/services-web-api](https://www.weather.gov/documentation/services-web-api)
- **Base URL:** `https://api.weather.gov`

#### Tags

- Weather
- Forecast
- Alerts
- Observations
- Aviation
- Hydrology
- GeoJSON

#### Properties

- [Documentation](https://www.weather.gov/documentation/services-web-api)
- [OpenAPI](https://api.weather.gov/openapi.json) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [OpenAPI](openapi/weather-gov-api-openapi.json) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/weather-gov-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/weather-gov-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [GitHub Repository](https://github.com/weather-gov/api)
- [Base U R L](https://api.weather.gov)
- [Changelog](https://www.weather.gov/documentation/services-web-api#/changelog)

### Space Weather Prediction Center (SWPC) Data Service

SWPC publishes solar wind, geomagnetic, X-ray flux, aurora forecast, radiation storm, and coronal mass ejection products through a static-file data service organised by format. JSON, text, and image feeds refresh on intervals from one minute (real-time solar wind) to daily summaries. No authentication required; products power aviation, satellite, power grid, GPS, and HAM radio operators. A modernization of the JSON catalog landed 2026-03-31 with old products deprecated 2026-04-30.

- **Human URL:** [https://www.swpc.noaa.gov/content/data-access](https://www.swpc.noaa.gov/content/data-access)
- **Base URL:** `https://services.swpc.noaa.gov`

#### Tags

- Space Weather
- Solar
- Geomagnetic
- Aurora
- Real-Time

#### Properties

- [Documentation](https://www.swpc.noaa.gov/content/data-access)
- [Base U R L](https://services.swpc.noaa.gov/json/)
- [Base U R L](https://services.swpc.noaa.gov/products/)
- [Base U R L](https://services.swpc.noaa.gov/text/)
- [Base U R L](https://services.swpc.noaa.gov/images/)
- [Changelog](https://www.swpc.noaa.gov/news/scn-upcoming-json-modifications-and-changes)
- [Postman Collection](collections/weather-gov-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/weather-gov-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### CO-OPS Data Retrieval API (Tides & Currents)

The Center for Operational Oceanographic Products and Services (CO-OPS) Data API returns water-level observations, tide predictions, currents, meteorological observations, and operational forecast model output (NOS OFS nowcasts) for over 200 stations along US coasts, the Great Lakes, and US territories. Supports XML, JSON, and CSV with selectable datums (MLLW, MHHW, MSL, plus Great Lakes datums), units, and time zones. Free, no key required. Stable endpoint at api.tidesandcurrents.noaa.gov.

- **Human URL:** [https://api.tidesandcurrents.noaa.gov/api/prod/](https://api.tidesandcurrents.noaa.gov/api/prod/)
- **Base URL:** `https://api.tidesandcurrents.noaa.gov/api/prod`

#### Tags

- Ocean
- Tides
- Currents
- Water Level
- Marine

#### Properties

- [Documentation](https://api.tidesandcurrents.noaa.gov/api/prod/)
- [Sandbox](https://tidesandcurrents.noaa.gov/api-helper/url-generator.html)
- [Documentation](https://tidesandcurrents.noaa.gov/products.html)
- [Postman Collection](collections/weather-gov-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/weather-gov-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### CO-OPS Metadata API (MDAPI v1)

The CO-OPS Metadata API exposes station inventory, harmonic constituents, NOS PORTS station lists, flood thresholds, and high/low water station catalogs. Supports radius and bounding-box station discovery and returns JSON or XML. Stable endpoint at api.tidesandcurrents.noaa.gov/mdapi/prod.

- **Human URL:** [https://api.tidesandcurrents.noaa.gov/mdapi/prod/](https://api.tidesandcurrents.noaa.gov/mdapi/prod/)
- **Base URL:** `https://api.tidesandcurrents.noaa.gov/mdapi/prod/webapi`

#### Tags

- Ocean
- Metadata
- Stations
- PORTS

#### Properties

- [Documentation](https://api.tidesandcurrents.noaa.gov/mdapi/prod/)
- [Changelog](https://api.tidesandcurrents.noaa.gov/mdapi/prod/releasenotes.html)
- [Postman Collection](collections/weather-gov-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/weather-gov-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### CO-OPS Derived Product API (DPAPI v0.1)

Derived products computed from historical CO-OPS water-level records — sea level trends, annual mean sea level reports, top-10 water levels, and extreme event summaries — exposed as a machine-readable companion to the data and metadata APIs.

- **Human URL:** [https://api.tidesandcurrents.noaa.gov/dpapi/prod/](https://api.tidesandcurrents.noaa.gov/dpapi/prod/)
- **Base URL:** `https://api.tidesandcurrents.noaa.gov/dpapi/prod`

#### Tags

- Ocean
- Sea Level
- Climate

#### Properties

- [Documentation](https://api.tidesandcurrents.noaa.gov/dpapi/prod/)
- [Postman Collection](collections/weather-gov-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/weather-gov-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### NCEI Access Data Service (v1)

The National Centers for Environmental Information (NCEI) Access Data Service is the modern, token-free replacement for the legacy CDO web service. It exposes daily summaries (GHCND), hourly summaries, monthly summaries, normals, global summaries of the day, sea-surface temperature, and many archived climate datasets. Returns CSV, JSON, NetCDF, or PDF. Stable endpoint at ncei.noaa.gov/access/services/data/v1.

- **Human URL:** [https://www.ncei.noaa.gov/support/access-data-service-api-user-documentation](https://www.ncei.noaa.gov/support/access-data-service-api-user-documentation)
- **Base URL:** `https://www.ncei.noaa.gov/access/services/data/v1`

#### Tags

- Climate
- Historical
- Stations
- GHCND

#### Properties

- [Documentation](https://www.ncei.noaa.gov/support/access-data-service-api-user-documentation)
- [Documentation](https://www.ncei.noaa.gov/access)
- [Postman Collection](collections/weather-gov-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/weather-gov-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### NCEI Climate Data Online (CDO) v2 API

The legacy Climate Data Online v2 REST API exposes datasets, datatypes, stations, locations, data categories, and observation records. Requires a free token from ncei.noaa.gov/cdo-web/token in the `token` header. Enforces 5 requests/second and 10,000 requests/day per token. Being superseded by the Access Data Service v1, but still widely deployed.

- **Human URL:** [https://www.ncdc.noaa.gov/cdo-web/webservices/v2](https://www.ncdc.noaa.gov/cdo-web/webservices/v2)
- **Base URL:** `https://www.ncei.noaa.gov/cdo-web/api/v2`

#### Tags

- Climate
- Historical
- Stations
- Datasets

#### Properties

- [Documentation](https://www.ncdc.noaa.gov/cdo-web/webservices/v2)
- [Authentication](https://www.ncdc.noaa.gov/cdo-web/token)
- [Rate Limits](rate-limits/noaa-gov-rate-limits.yml)
- [Postman Collection](collections/weather-gov-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/weather-gov-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### National Data Buoy Center (NDBC) Web Data Service

NDBC publishes real-time meteorological and oceanographic observations (the last 45 days) and historical archives from a global network of over 900 moored buoys, drifting buoys, C-MAN coastal stations, and partner stations. Data is exposed via HTTP file URLs, a THREDDS Data Server, and an OGC API Features collection. Observations include wave height, period, direction, sea surface temperature, wind, air pressure, salinity, and visibility.

- **Human URL:** [https://www.ndbc.noaa.gov/docs/ndbc_web_data_guide.pdf](https://www.ndbc.noaa.gov/docs/ndbc_web_data_guide.pdf)
- **Base URL:** `https://www.ndbc.noaa.gov/data`

#### Tags

- Ocean
- Marine
- Buoys
- Waves
- Observations

#### Properties

- [Documentation](https://www.ndbc.noaa.gov/docs/ndbc_web_data_guide.pdf)
- [Documentation](https://www.ndbc.noaa.gov/faq/rt_data_access.shtml)
- [Documentation](https://www.ndbc.noaa.gov/thredds/catalog.html)
- [Postman Collection](collections/weather-gov-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/weather-gov-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### NOAA CoastWatch ERDDAP Server

ERDDAP (Environmental Research Division Data Access Program) is a NOAA-funded, open-source server that unifies access to gridded (`griddap`) and tabular (`tabledap`) scientific datasets across OPeNDAP, WMS, and REST. CoastWatch, ERD/PFEG, NCEI, IOOS, and many NOAA line offices each operate ERDDAP instances exposing tens of thousands of datasets (satellite SST, chlorophyll, ocean color, altimetry, model output, in-situ observations) in CSV, JSON, NetCDF, MATLAB, Parquet, and image formats.

- **Human URL:** [https://coastwatch.pfeg.noaa.gov/erddap/information.html](https://coastwatch.pfeg.noaa.gov/erddap/information.html)
- **Base URL:** `https://coastwatch.pfeg.noaa.gov/erddap`

#### Tags

- Ocean
- Satellite
- Climate
- Scientific Data
- OPeNDAP

#### Properties

- [Documentation](https://coastwatch.pfeg.noaa.gov/erddap/information.html)
- [Documentation](https://coastwatch.pfeg.noaa.gov/erddap/rest.html)
- [Documentation](https://coastwatch.pfeg.noaa.gov/erddap/griddap/documentation.html)
- [Base U R L](https://www.ncei.noaa.gov/erddap/)
- [Base U R L](https://coastwatch.noaa.gov/erddap/)
- [Postman Collection](collections/weather-gov-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/weather-gov-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### NOAA Open Data Dissemination (NODD)

NODD is NOAA's bulk-data dissemination program, providing free, low-latency public access to tens of terabytes per day of forecast model output, satellite imagery, radar, and observation archives through public-private partnerships with AWS, Google Cloud, and Microsoft Azure. Datasets include GFS, GEFS, HRRR, RAP, NAM, RRFS, GraphCast, GOES-16/17/18/19, NEXRAD Level II/III, and hundreds of climate archives — all addressable as S3/GCS/Azure Blob objects, without keys.

- **Human URL:** [https://www.noaa.gov/information-technology/open-data-dissemination](https://www.noaa.gov/information-technology/open-data-dissemination)
- **Base URL:** `https://noaa-gfs-bdp-pds.s3.amazonaws.com`

#### Tags

- Open Data
- Cloud
- Bulk Data
- Forecast Models
- Satellite
- Radar

#### Properties

- [Documentation](https://www.noaa.gov/information-technology/open-data-dissemination)
- [Documentation](https://www.noaa.gov/nodd/datasets)
- [Documentation](https://registry.opendata.aws/collab/noaa/)
- [Base U R L](https://registry.opendata.aws/noaa-gfs-bdp-pds/)
- [Base U R L](https://registry.opendata.aws/noaa-hrrr-pds/)
- [Base U R L](https://registry.opendata.aws/noaa-gefs/)
- [Base U R L](https://registry.opendata.aws/noaa-space-weather/)
- [Postman Collection](collections/weather-gov-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/weather-gov-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### NOAA Fisheries One Stop Shop (FOSS) ODS / ORDS

The Fisheries One Stop Shop (FOSS) Operational Data Store, hosted on Oracle REST Data Services (ORDS), exposes US commercial fisheries landings, foreign trade, fishing gear, and species reference data. Cloud-hosted at apps-st.fisheries.noaa.gov with a public metadata catalog and paginated REST endpoints; suitable for fisheries economics, stock assessment, and policy analysis.

- **Human URL:** [https://www.fisheries.noaa.gov/foss/f?p=215:35](https://www.fisheries.noaa.gov/foss/f?p=215:35)
- **Base URL:** `https://apps-st.fisheries.noaa.gov/ods/foss`

#### Tags

- Fisheries
- Landings
- Marine
- Trade
- Reference Data

#### Properties

- [Documentation](https://www.fisheries.noaa.gov/foss/f?p=215:35)
- [Documentation](https://apps-st.fisheries.noaa.gov/ods/foss/metadata-catalog/?offset=0&limit=100)
- [Documentation](https://www.fisheries.noaa.gov/inport/item/10574)
- [Postman Collection](collections/weather-gov-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/weather-gov-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### NOAA InPort Metadata Catalog

InPort is the authoritative metadata repository for NOAA Fisheries and the National Ocean Service and the NOAA-wide platform for data management plans. Catalog records describe data products, services, projects, and contacts; the public-facing site supports search and item retrieval, while web service endpoints support catalog-item path lookup and contact management. Public API endpoints are stabilising — full machine-to-machine surface is in beta.

- **Human URL:** [https://www.fisheries.noaa.gov/inport/](https://www.fisheries.noaa.gov/inport/)
- **Base URL:** `https://www.fisheries.noaa.gov/inport`

#### Tags

- Metadata
- Catalog
- Fisheries
- Ocean

#### Properties

- [Documentation](https://www.fisheries.noaa.gov/inport/)
- [Changelog](https://www.fisheries.noaa.gov/inport/release-notes)
- [Postman Collection](collections/weather-gov-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/weather-gov-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [Portal](https://www.noaa.gov/)
- [Documentation](https://www.noaa.gov/organization)
- [Documentation](https://www.noaa.gov/information-technology/open-data-dissemination)
- [Documentation](https://catalog.data.gov/organization/noaa-gov)
- [Portal](https://data.noaa.gov/)
- [Documentation](https://www.noaa.gov/foia)
- [Terms of Service](https://www.noaa.gov/legal)
- [Privacy Policy](https://www.noaa.gov/privacy-policy)
- [Blog](https://www.noaa.gov/news)
- [Blog](https://www.weather.gov/news)
- [Blog](https://www.swpc.noaa.gov/news)
- [Support](https://www.weather.gov/contact)
- [Support](https://www.ncei.noaa.gov/contact)
- [Documentation](https://www.noaa.gov/jobs)
- [GitHub Organization](https://github.com/NOAA-EMC)
- [GitHub Organization](https://github.com/NOAA-GFDL)
- [GitHub Organization](https://github.com/NOAA-GSL)
- [GitHub Organization](https://github.com/NOAA-OWP)
- [GitHub Organization](https://github.com/NOAA-PSL)
- [GitHub Organization](https://github.com/NOAA-PMEL)
- [GitHub Organization](https://github.com/NOAAGFDL)
- [GitHub Organization](https://github.com/weather-gov)
- [GitHub Repository](https://github.com/weather-gov/api)
- [GitHub Repository](https://github.com/weather-gov/weather.gov)
- [GitHub Repository](https://github.com/NOAA-EMC/global-workflow)
- [GitHub Repository](https://github.com/NOAA-GSL/Rocoto)
- [Documentation](https://www.weather.gov/sti/)
- [Documentation](https://www.weather.gov/about/who-we-are)
- [Portal](https://www.nesdis.noaa.gov/)
- [Portal](https://oceanservice.noaa.gov/)
- [Portal](https://www.fisheries.noaa.gov/)
- [Portal](https://research.noaa.gov/)
- [Portal](https://www.omao.noaa.gov/)
- [Portal](https://www.ncei.noaa.gov/)
- [Base U R L](https://www.ncei.noaa.gov/erddap/)
- [JSON-LD](https://json-ld/noaa-gov-context.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)
- [Vocabulary](https://vocabulary/noaa-gov-vocabulary.yml)
- [Rate Limits](https://rate-limits/noaa-gov-rate-limits.yml)
- [Features](undefined)

## Maintainers

**FN:** Kin Lane
**Email:** info@apievangelist.com
**URL:** https://apievangelist.com
