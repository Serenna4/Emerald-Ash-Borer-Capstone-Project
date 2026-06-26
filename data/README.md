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

- **Source:** https://geohub.oregon.gov/datasets/oregon-geo::historic-vegetation/explore?location=44.114174%2C-120.514863%2C7&showTable=true
- **License:** CC0 1.0 License: The person who associated a work with this deed has dedicated the work to the public domain by waiving all of his or her rights to the work worldwide under copyright law, including all related and neighboring rights, to the extent allowed by law. You can copy, modify, distribute and perform the work, even for commercial purposes, all without asking permission. See Other Information below.
- **Date pulled:** <2026-06-22>
- **Approximate size:** shapefile, rows: 43,628, columns: 2, bytes: 150,272 KB
- **Owner on this project:** State of Oregon, hosted on GEOHub Data
- **Where it lives in this repo:** Currently the file is too large to be hosted on Github. 
- **Ethics / consent notes:** There is no PII and no concent concerns. We are more concerned that this data may not contain the exact locations of Salem's smaller streams which is necessary for our research. 
- **How to fetch (for a teammate cloning fresh):** Download the file from the source link. The data was last updated June 27, 2023. 

### Dataset 3: Address Density

- **Source:** https://data.cityofsalem.net/datasets/d686030c3b1a474bbe019320b77ce7e6_0/explore?location=44.939875%2C-123.027427%2C13 
- **License:** This product has been prepared by Salem GIS professionals for use by Salem staff and as a reference for online users.  This product is provided as is, without warranty, for informational purposes only.  The City makes no warranty, representation, or guaranty of completeness, accuracy, content or fitness for any particular use.  Products have been prepared for specific city purposes and may not be appropriate for all other uses.  The City is not responsible for any errors, omission, or inaccuracies in the products provided. Development of derivative products is encouraged however copying and selling the data is prohibited.  The City reserves the right to discontinue availability of content at any time and for any reason.  In no event is the City of Salem liable for damages from the use of this product.  Contact the Salem IT Department for more information at gis@cityofsalem.net
- **Date pulled:** <2026-06-23>
- **Approximate size:** rows: 93,164, columns: 44, bytes: 31,582 KB
- **Owner on this project:** City of Salem Oregon GIS
- **Where it lives in this repo:** Currently the file is too large to be hosted on Github. 
- **Ethics / consent notes:** My only concern would be that some Salem residents would feel uncomfortable seeing their exact address in a project, even without any PII connected to it. To prevent any concerns in this regard, we will aggregate this data into the number of addresses in each Salem zipcode. 
- **How to fetch (for a teammate cloning fresh):** Download the file from the source link.

### Dataset 4: <name>

- **Source:** <URL or contact>
- **License:** <name and short summary>
- **Date pulled:** <YYYY-MM-DD>
- **Approximate size:** <rows, columns, bytes>
- **Owner on this project:** <name>
- **Where it lives in this repo:** `data/raw/<name>/` (gitignored) or `data/processed/<name>.csv`
- **Ethics / consent notes:** <PII? consent process? data use agreement?>
- **How to fetch (for a teammate cloning fresh):** <command, script, or contact>

### Dataset 5: <name>

- **Source:** <URL or contact>
- **License:** <name and short summary>
- **Date pulled:** <YYYY-MM-DD>
- **Approximate size:** <rows, columns, bytes>
- **Owner on this project:** <name>
- **Where it lives in this repo:** `data/raw/<name>/` (gitignored) or `data/processed/<name>.csv`
- **Ethics / consent notes:** <PII? consent process? data use agreement?>
- **How to fetch (for a teammate cloning fresh):** <command, script, or contact>

### Dataset 6: <name>

- **Source:** <URL or contact>
- **License:** <name and short summary>
- **Date pulled:** <YYYY-MM-DD>
- **Approximate size:** <rows, columns, bytes>
- **Owner on this project:** <name>
- **Where it lives in this repo:** `data/raw/<name>/` (gitignored) or `data/processed/<name>.csv`
- **Ethics / consent notes:** <PII? consent process? data use agreement?>
- **How to fetch (for a teammate cloning fresh):** <command, script, or contact>

### Dataset 7: <name>

- **Source:** <URL or contact>
- **License:** <name and short summary>
- **Date pulled:** <YYYY-MM-DD>
- **Approximate size:** <rows, columns, bytes>
- **Owner on this project:** <name>
- **Where it lives in this repo:** `data/raw/<name>/` (gitignored) or `data/processed/<name>.csv`
- **Ethics / consent notes:** <PII? consent process? data use agreement?>
- **How to fetch (for a teammate cloning fresh):** <command, script, or contact>

