# NOAA — National Oceanic and Atmospheric Administration (noaa-gov)

The National Oceanic and Atmospheric Administration (NOAA) is the United States scientific and regulatory agency within the Department of Commerce charged with monitoring oceanic and atmospheric conditions, charting the seas, conducting deep-sea exploration, managing fishing and protection of marine mammals, and providing weather, climate, space weather, and ecosystem forecasts and warnings.

NOAA's developer surface spans six line offices — the National Weather Service (NWS), the National Environmental Satellite, Data, and Information Service (NESDIS) including the National Centers for Environmental Information (NCEI), the National Ocean Service (NOS) including Tides & Currents (CO-OPS), the National Marine Fisheries Service (NMFS / NOAA Fisheries), the Office of Oceanic and Atmospheric Research (OAR), and the Office of Marine and Aviation Operations (OMAO). NOAA exposes free, open APIs at `api.weather.gov`, `services.swpc.noaa.gov`, `api.tidesandcurrents.noaa.gov`, `ncei.noaa.gov/access`, ERDDAP servers across line offices, the National Data Buoy Center (NDBC), and bulk forecast model output (GFS, GEFS, HRRR, GOES) through the NOAA Open Data Dissemination (NODD) program on AWS, GCP, and Azure.

**URL:** [Visit APIs.json](https://raw.githubusercontent.com/api-evangelist/noaa-gov/refs/heads/main/apis.yml)

**Review:** Tier 1 — comprehensive open developer surface. See [review.yml](review.yml).

## Tags

- Weather, Climate, Ocean, Space Weather, Government, Open Data, Forecast, Marine, Atmospheric, Hydrology, Satellite, Fisheries, Aviation, Emergency Management

## Timestamps

- **Created:** 2026-05-25
- **Modified:** 2026-05-25

## APIs

### National Weather Service API (api.weather.gov)
The public NWS REST API delivers real-time forecasts, alerts (CAP), observations, gridded forecast data, aviation products, and metadata for offices, zones, and radar stations across the US and US territories. GeoJSON by default with content negotiation for JSON-LD, CAP, ATOM, and DWML. No API key — only a User-Agent. OpenAPI 3.9.2, 66 documented paths.

**Human URL:** [https://www.weather.gov/documentation/services-web-api](https://www.weather.gov/documentation/services-web-api)

- [Documentation](https://www.weather.gov/documentation/services-web-api)
- [OpenAPI (live)](https://api.weather.gov/openapi.json)
- [OpenAPI (mirrored)](openapi/weather-gov-api-openapi.json)
- [GitHub — weather-gov/api](https://github.com/weather-gov/api)

### Space Weather Prediction Center (SWPC) Data Service
Solar wind, geomagnetic, X-ray flux, aurora, and CME products as JSON, text, and image feeds. No authentication. JSON catalog modernised 2026-03-31.

**Human URL:** [https://www.swpc.noaa.gov/content/data-access](https://www.swpc.noaa.gov/content/data-access)

- [JSON Feeds](https://services.swpc.noaa.gov/json/)
- [Text Feeds](https://services.swpc.noaa.gov/text/)
- [Products](https://services.swpc.noaa.gov/products/)

### CO-OPS Data Retrieval API (Tides & Currents)
Water-level observations, tide predictions, currents, meteorological observations, and NOS OFS nowcasts for 200+ coastal, Great Lakes, and territorial stations. XML, JSON, CSV. Selectable datums (MLLW, MHHW, MSL, Great Lakes).

**Human URL:** [https://api.tidesandcurrents.noaa.gov/api/prod/](https://api.tidesandcurrents.noaa.gov/api/prod/)

### CO-OPS Metadata API (MDAPI v1)
Station inventory, harmonic constituents, PORTS lists, flood thresholds, high/low water station catalogs. Radius and bounding-box discovery.

**Human URL:** [https://api.tidesandcurrents.noaa.gov/mdapi/prod/](https://api.tidesandcurrents.noaa.gov/mdapi/prod/)

### CO-OPS Derived Product API (DPAPI v0.1)
Sea-level trends, annual mean sea level reports, top-10 water levels, extreme event summaries.

**Human URL:** [https://api.tidesandcurrents.noaa.gov/dpapi/prod/](https://api.tidesandcurrents.noaa.gov/dpapi/prod/)

### NCEI Access Data Service (v1)
Token-free climate data — GHCND daily, hourly, monthly, normals, SST archives. CSV, JSON, NetCDF, PDF.

**Human URL:** [https://www.ncei.noaa.gov/support/access-data-service-api-user-documentation](https://www.ncei.noaa.gov/support/access-data-service-api-user-documentation)

### NCEI Climate Data Online (CDO) v2 API
Legacy token-based REST API. 5 req/sec, 10,000 req/day per token.

**Human URL:** [https://www.ncdc.noaa.gov/cdo-web/webservices/v2](https://www.ncdc.noaa.gov/cdo-web/webservices/v2)

- [Token request](https://www.ncdc.noaa.gov/cdo-web/token)
- [Rate limits](rate-limits/noaa-gov-rate-limits.yml)

### National Data Buoy Center (NDBC) Web Data Service
Real-time (last 45 days) and historical observations from 900+ moored buoys, drifting buoys, C-MAN stations, and partner platforms. HTTP files, THREDDS, OGC API Features.

**Human URL:** [https://www.ndbc.noaa.gov/docs/ndbc_web_data_guide.pdf](https://www.ndbc.noaa.gov/docs/ndbc_web_data_guide.pdf)

### NOAA CoastWatch ERDDAP Server
Unified REST access to gridded (`griddap`) and tabular (`tabledap`) scientific datasets across satellites, models, and in-situ observations. CSV, JSON, NetCDF, MATLAB, Parquet.

**Human URL:** [https://coastwatch.pfeg.noaa.gov/erddap/information.html](https://coastwatch.pfeg.noaa.gov/erddap/information.html)

- [REST docs](https://coastwatch.pfeg.noaa.gov/erddap/rest.html)
- [NCEI ERDDAP](https://www.ncei.noaa.gov/erddap/)
- [CoastWatch (national)](https://coastwatch.noaa.gov/erddap/)

### NOAA Open Data Dissemination (NODD)
Multi-cloud bulk-data program. GFS, GEFS, HRRR, RAP, NAM, RRFS, GraphCast, GOES-16/17/18/19, NEXRAD Level II/III on AWS, GCP, and Azure. No keys.

**Human URL:** [https://www.noaa.gov/information-technology/open-data-dissemination](https://www.noaa.gov/information-technology/open-data-dissemination)

- [Dataset list](https://www.noaa.gov/nodd/datasets)
- [AWS registry](https://registry.opendata.aws/collab/noaa/)

### NOAA Fisheries One Stop Shop (FOSS) ODS / ORDS
US commercial fisheries landings, foreign trade, gear, and species reference data via Oracle REST Data Services.

**Human URL:** [https://www.fisheries.noaa.gov/foss/f?p=215:35](https://www.fisheries.noaa.gov/foss/f?p=215:35)

- [Metadata catalog](https://apps-st.fisheries.noaa.gov/ods/foss/metadata-catalog/?offset=0&limit=100)

### NOAA InPort Metadata Catalog
Authoritative metadata repository for NOAA Fisheries and NOS. Catalog records cover data products, services, projects, and contacts.

**Human URL:** [https://www.fisheries.noaa.gov/inport/](https://www.fisheries.noaa.gov/inport/)

## Artifacts

- [apis.yml](apis.yml) — APIs.json 0.19 catalog
- [openapi/weather-gov-api-openapi.json](openapi/weather-gov-api-openapi.json) — NWS API OpenAPI 3.9.2
- [json-schema/noaa-gov-alert-schema.json](json-schema/noaa-gov-alert-schema.json) — NWS Alert (CAP) JSON Schema
- [json-ld/noaa-gov-context.jsonld](json-ld/noaa-gov-context.jsonld) — JSON-LD context for NOAA APIs
- [vocabulary/noaa-gov-vocabulary.yml](vocabulary/noaa-gov-vocabulary.yml) — Controlled vocabulary across line offices, products, models, formats
- [rate-limits/noaa-gov-rate-limits.yml](rate-limits/noaa-gov-rate-limits.yml) — Documented rate-limit policies
- [review.yml](review.yml) — API Evangelist review (Tier 1)

## GitHub Organizations

- [weather-gov](https://github.com/weather-gov) — NWS API + weather.gov 2.0
- [NOAA-EMC](https://github.com/NOAA-EMC) — Environmental Modeling Center (GFS, GEFS workflows)
- [NOAA-GFDL](https://github.com/NOAA-GFDL) — Geophysical Fluid Dynamics Laboratory
- [NOAA-GSL](https://github.com/NOAA-GSL) — Global Systems Laboratory (HRRR, RRFS, Rocoto)
- [NOAA-OWP](https://github.com/NOAA-OWP) — Office of Water Prediction
- [NOAA-PMEL](https://github.com/NOAA-PMEL) — Pacific Marine Environmental Laboratory
- [NOAA-PSL](https://github.com/NOAA-PSL) — Physical Sciences Laboratory

## Maintainer

- Kin Lane — [API Evangelist](https://apievangelist.com)
