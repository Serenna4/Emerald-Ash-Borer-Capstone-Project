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

- **Source:** Sent to us by Meredith from the City of Salem 
- **License:** CC0 1.0 License: The person who associated a work with this deed has dedicated the work to the public domain by waiving all of his or her rights to the work worldwide under copyright law, including all related and neighboring rights, to the extent allowed by law. You can copy, modify, distribute and perform the work, even for commercial purposes, all without asking permission. See Other Information below.
- **Date pulled:** <2026-05-27>
- **Approximate size:** rows: 589,645, columns: 5, bytes: 25,653 KB
- **Owner on this project:** City of Salem
- **Where it lives in this repo:** `data/processed/Seasonal_Temp_Loggers.csv`
- **Ethics / consent notes:** There is no PII and no consert concerns. We should be wary that this data only spans from  2018-05-01 to 2022-10-04 and that we should be cautious extrapolating any findings outside of this time range. 
- **How to fetch (for a teammate cloning fresh):** Contact Meredith Greer at <MGreer@cityofsalem.net>

### Dataset 2: Stream Location Data

- **Source:** https://data.cityofsalem.net/datasets/073807388cb64c828a43897933e770ce/explore?location=44.926409%2C-122.919209%2C10&showTable=true
- **License:** Custom License: The data in SalemMaps Online has been prepared for use by GIS professionals and as a reference map for online users. For official City of Salem information and maps, please go to https://www.cityofsalem.net This product is provided as is, without warranty. In no event is the City of Salem liable for damages from the use of this product. The data in this product is subject to license and copyright limitations and further distribution or resale is governed by licensing restrictions. Contact the Salem IT Department for more information at gis@cityofsalem.net
- **Date pulled:** <2026-06-26>
- **Approximate size:** shapefile, rows: 2,672, columns: 24, bytes: 619 KB
- **Owner on this project:** City of Salem, Oregon
- **Where it lives in this repo:**  `data/processed/Public_Storm_Creeks_and_Rivers_4477802176423454413.zip`
- **Ethics / consent notes:** There is no PII and no concent concerns.
- **How to fetch (for a teammate cloning fresh):** Download the file from the source link. The data was last updated May 30, 2026. 

### Dataset 3: Addresses by Zipcode

- **Source:** https://data.cityofsalem.net/datasets/d686030c3b1a474bbe019320b77ce7e6_0/explore?location=44.939875%2C-123.027427%2C13 
- **License:** This product has been prepared by Salem GIS professionals for use by Salem staff and as a reference for online users.  This product is provided as is, without warranty, for informational purposes only.  The City makes no warranty, representation, or guaranty of completeness, accuracy, content or fitness for any particular use.  Products have been prepared for specific city purposes and may not be appropriate for all other uses.  The City is not responsible for any errors, omission, or inaccuracies in the products provided. Development of derivative products is encouraged however copying and selling the data is prohibited.  The City reserves the right to discontinue availability of content at any time and for any reason.  In no event is the City of Salem liable for damages from the use of this product.  Contact the Salem IT Department for more information at gis@cityofsalem.net
- **Date pulled:** <2026-06-23>
- **Approximate size:** rows: 93,164, columns: 44, bytes: 31,582 KB
- **Owner on this project:** City of Salem Oregon GIS
- **Where it lives in this repo:** Currently the file is too large to be hosted on Github. 
- **Ethics / consent notes:** My only concern would be that some Salem residents would feel uncomfortable seeing their exact address in a project, even without any PII connected to it. To prevent any concerns in this regard, we will aggregate this data into the number of addresses in each Salem zipcode. 
- **How to fetch (for a teammate cloning fresh):** Download the file from the source link.

### Dataset 4: Zipcode Population and Area

- **Source:** https://censusreporter.org/
- **License:** The information is a free, open-source project. Additionally, Census data is always free and public. More information at: https://censusreporter.org/about/
- **Date pulled:** <2026-06-25>
- **Approximate size:** rows: 7, columns: 2
- **Owner on this project:** Census Reporter
- **Where it lives in this repo:**  `data/processed/zip_density.csv`
- **Ethics / consent notes:** This data is open source and aggregated so there is no PII. 
- **How to fetch (for a teammate cloning fresh):** Information is included in the RMarkdown and will automatically be added to the Addresses by Zipcode file. 

### Dataset 5: EAB Infestation Areas

- **Source:** https://experience.arcgis.com/experience/9f29b1860cb04d36ad71b122148277f3/page/Page
- **License:** This work is licensed under CC BY-SA 4.0
- **Date pulled:** 2026-06-28
- **Approximate size:** <rows, columns, bytes>
- **Owner on this project:** Oregon Department of Forestry
- **Where it lives in this repo:** `data/raw/eab.csv/`
- **Ethics / consent notes:** Since we are only collecting the EAB infestation zones, there is no PII in this data. This is also public information so it can be shared freely. 
- **How to fetch (for a teammate cloning fresh):** Access through the script to web scrape the data or through the file in the `data/raw/eab.csv/`

### Dataset 6: Tree Plotter

- **Source:** https://pg-cloud.com/Oregon/
- **License:** The Oregon Department of Forestry’s Urban and Community Forestry Program has made the TreePlotter inventory and canopy assessment tools available for use at no cost to community partners throughout the state.
- **Date pulled:** <YYYY-MM-DD> (not pulled yet)
- **Approximate size:** rows: , columns: , bytes: 
- **Owner on this project:** Oregon Department of Forestry
- **Where it lives in this repo:** `data/raw/tree.csv/` 
- **Ethics / consent notes:** This information is publicly available and contains no PII. It is clear that this data is free to use for projects so there are not use agreements. 
- **How to fetch (for a teammate cloning fresh):** Data was scraped using a web scraping script. 

### Dataset 7: Weather Data

- **Source:** https://www.ncdc.noaa.gov/cdo-web/search;jsessionid=8DC3FCE6E9A0F7A195852DFB26D8632A
- **License:** License information is not readily available on the website however the data is openly available and is meant for use by researchers. 
- **Date pulled:** 2026-06-14
- **Approximate size:** rows: 48603, columns: 18, bytes: 15.1 MB
- **Owner on this project:** NOAA, USA.gov
- **Where it lives in this repo:** `data/raw/USW00024232.csv/` 
- **Ethics / consent notes:** This information is public and contains no PII. This can be used openly. 
- **How to fetch (for a teammate cloning fresh):** Data can be downloaded from the source url or be found in `data/raw/USW00024232.csv/` 
