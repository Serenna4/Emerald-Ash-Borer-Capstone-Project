# `data/`

Project data lives here. The repo root `.gitignore` excludes large or sensitive subfolders by default. The structure below is the convention you should follow.

```
data/
  raw/         # original inputs, never edited in place        (gitignored)
  external/    # third-party data you did not generate         (gitignored)
  interim/     # intermediate scratch outputs                  (gitignored)
  processed/   # cleaned, analysis-ready snapshots (committable if small)
  README.md    # describe each dataset: source, license, date, size
  SCHEMA.md    # describe processed dataset schemas once they stabilize
```

## What to **always** commit

- This `README.md` describing every dataset, with: source URL or contact, license, date pulled, approximate size, who in the team owns it, and any ethics / consent notes.
- A `SCHEMA.md` documenting the columns, types, and units of your processed datasets, once they stabilize.
- Small (< 1 MB) reproducible processed snapshots under `data/processed/` if your analysis depends on a specific version.

## What to **never** commit

- Personally identifiable information (PII), protected health information (PHI), or any data subject to a data use agreement that forbids redistribution.
- Credentials, API keys, OAuth tokens, or `.env` files.
- Multi-megabyte raw downloads. Document how to fetch them in this README instead.

## Dataset registry (fill in)

### Dataset 1: Stream Temperature Data

- **Source:** Sent to us by Dr. Gore from Willamette University. Data collection project launched in 2025 by CastawayWU. https://sites.google.com/willamette.edu/castaway-club/mill-creek-research-project
- **License:** Available by request.
- **Date pulled:** <2026-06-29>
- **Approximate size:** rows: 7,543, columns: 5, bytes: 426 KB
- **Owner on this project:** CastawayWU
- **Where it lives in this repo:** `data/raw/ds_daily.csv`
- **Ethics / consent notes:** There is no PII and no consert concerns. We should be wary that this data only spans from  014-12-31 to 2025-6-4 and that we should be cautious extrapolating any findings outside of this time range. 
- **How to fetch (for a teammate cloning fresh):** Contact CastawayWU at from their contact page on the source link.

### Dataset 2: Stream Location Data

- **Source:** https://data.cityofsalem.net/datasets/073807388cb64c828a43897933e770ce/explore?location=44.926409%2C-122.919209%2C10&showTable=true
- **License:** Custom License: The data in SalemMaps Online has been prepared for use by GIS professionals and as a reference map for online users. For official City of Salem information and maps, please go to https://www.cityofsalem.net This product is provided as is, without warranty. In no event is the City of Salem liable for damages from the use of this product. The data in this product is subject to license and copyright limitations and further distribution or resale is governed by licensing restrictions. Contact the Salem IT Department for more information at gis@cityofsalem.net
- **Date pulled:** <2026-06-26>
- **Approximate size:** shapefile, rows: 2,672, columns: 24, bytes: 619 KB
- **Owner on this project:** City of Salem, Oregon
- **Where it lives in this repo:**  `data/processed/Public_Storm_Creeks_and_Rivers_4477802176423454413.zip`
- **Ethics / consent notes:** There is no PII and no concent concerns.
- **How to fetch (for a teammate cloning fresh):** Download the file from the source link. The data was last updated May 30, 2026. 

### Dataset 3: Weather Data

- **Source:** https://www.ncdc.noaa.gov/cdo-web/search;jsessionid=8DC3FCE6E9A0F7A195852DFB26D8632A
- **License:** License information is not readily available on the website however the data is openly available and is meant for use by researchers. 
- **Date pulled:** 2026-06-14
- **Approximate size:** rows: 48603, columns: 18, bytes: 15.1 MB
- **Owner on this project:** NOAA, USA.gov
- **Where it lives in this repo:** `data/raw/USW00024232.csv/` 
- **Ethics / consent notes:** This information is public and contains no PII. This can be used openly. 
- **How to fetch (for a teammate cloning fresh):** Data can be downloaded from the source url or be found in `data/raw/USW00024232.csv/` 
