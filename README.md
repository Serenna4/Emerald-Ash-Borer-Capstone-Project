# Protecting Salem’s Ecosystem by Preventing the Spread of the Emerald Ash Borer

Analyzing the impact of Emerald Ash Borer infestations, high risk forested areas, and the impact of dying Ash Trees in Salem, OR. 

## Quick reference

| Field | Value |
|-------|-------|
| Owner team | Siera Edwards, Serenna Walter, and Brooke Proctor |
| Owner Product Lead | Serenna Walter |
| Peer Stakeholder POs | Amaya Supancich-McCord, Spencer Fiden |
| Studio Session | 3 |
| GitHub repo | https://github.com/Serenna4/Emerald-Ash-Borer-Capstone-Project |
| GitHub Projects board | https://github.com/users/Serenna4/projects/2 |
| Discord category | `#Project 21` |
| Instructor / Sponsor | Lucas Cordova (`LucasCordova` on GitHub) |

## What this repo contains

| Path | Purpose |
|------|---------|
| [`CHARTER.md`](CHARTER.md) | Studio Charter: vision, mission, context, success criteria, working agreements, SLAs, DoR / DoD. Committed at the end of the week 3 Studio Charter session. |
| [`BACKLOG.md`](BACKLOG.md) | Human-readable mirror of the GitHub Projects board. |
| [`studio/briefs/`](studio/briefs/) | Weekly Studio Briefs from peer POs (`W<NN>-<peer>.md`). |
| [`studio/critiques/`](studio/critiques/) | Weekly Studio Critiques from peer POs (`W<NN>-<peer>.md`). |
| [`src/`](src/) | Working code (scripts, modules). |
| [`notebooks/`](notebooks/) | Exploratory and reporting notebooks. |
| [`data/`](data/) | Project data. Raw inputs are `.gitignored` by default; see `data/README.md`. |
| [`deliverables/`](deliverables/) | Milestone deliverables: proposal, data summary, poster, write-up. |

## How this project runs (DS3 in one paragraph)

This project is run as a **DS3 studio**: the owner team is paired with two or three **peer Stakeholder POs** drawn from adjacent capstone projects. Every week the peer POs file a **Studio Brief** for the next iteration and a **Studio Critique** of the last iteration. The owner team commits an **Iteration Review** here in `README.md` before each class. See the [Studio Session weekly ritual](https://courses.lpcordova.phd/data510/project-framework/weekly-ritual.html) for the cadence and [Studio Charter](https://courses.lpcordova.phd/data510/project-framework/charter-inception.html) for the inception session.

---

# Iteration Reviews

One subsection per class week. The owner team commits the new section **before each class** so peer POs can read it before filing the next Brief and Critique. Use the template at the bottom of this file for any extra weeks you add.

## Week 4 -- Proposal milestone (M1)

**Iteration ending:** 5/30/2026
**Milestone tag in focus:** `M1-proposal`

**Completed PBIs**
- Milestone One Proposal

**In-flight (carrying across the boundary)**
- Everything Else
- Data Cleaning
- Select Which Datasets to Use
- Collect Data
- Reach out to Meridith
- Assign Directions for Each of Us
- Finish Charter Document Touchups
- Aquire and Document
- Create Data Engineering Plan
- Draft research question and frame as a testable claim

**Stakeholder response log**
- Studio Brief from <peer PO 1>: adopted = ..., deferred = ..., declined (with reason) = ...
- Studio Brief from <peer PO 2>: adopted = ..., deferred = ..., declined (with reason) = ...

**Plan for next iteration**
- Top PBIs (with milestone tags):
- Acquire and document (M2)
- Reach out to Meridith
- Move to analyze:
    - Draft Research Question
    - Data Engineering Plan

**Risks and impediments**
- Need to acquire data quickly with a webscraper. May need support from Professor Cordova.

## Week 5

**Iteration ending:** 6/8/2026
**Milestone tag in focus:** `M1-proposal` / `M2-data-summary`

**Completed PBIs**
- Finish Charter Document Touchups
- Draft research question and frame as a testable claim
- Assign directions for each of us.
- Create Data Engineering Plan
- Set up Railway for this project
- Email Meridith

**Stakeholder response log**
- No feedback yet. 

**Plan for next iteration**
- Collect Data using web scrapers
- Collect Data not needing web scrapers
- Select Which Datasets to Use
- Data Cleaning
- Move data into Railway

**Risks and impediments**
- We beileve we will have to use web scraping to gather some of the map data. So far we are having trouble with collecting the latitude and longitude information.

## Week 6

**Iteration ending:** 6/15/2026
**Milestone tag in focus:**  `M1-proposal` / `M2-data-summary`

**Completed PBIs**
- Collect Data using web scrapers
- Collect Data not needing web scrapers
- Select Which Datasets to Use

**Stakeholder response log**
- No feedback yet. We will get Project Proposal Feedback in the next couple days. 

**Plan for next iteration**
- Use feedback from Peer POs to improve Project Proposal
- Clean all datasets 
- Get datasets into usable formats
- Add data files to the appropriate Github folders
- Start filling out Data Summary Documentation

**Risks and impediments**
- There is a risk that our data will not actually be in the format we need when we open it and start cleaning.
- We may find that these datasets do not answer our research questions but this risk is low. If this happens, we can check out our other reserved datasets and see if they are more fitting. 

## Week 7 -- Data summary milestone (M2)

**Iteration ending:** 6/22/2026
**Milestone tag in focus:** `M2-data-summary`

**Completed PBIs**
- Select final data sources
- Serenna: Clean EAB data
- Siera: Clean stream temperature data
- Siera: Clean and aggregate home density data
- Brooke: Clean temperature data

**Stakeholder response log**
- Project Proposal Feedback: We got a lot of positive feedback on our project proposal. Some critiques we want to implement include writing more contextual information about rising water temperatures and meaking a clearer data engineering design. Our peers mentioned that it was difficult to tell exactly what we are joining all our data on, however, we plan on having separate datasets for different models and not all data will be joined. 

**Plan for next iteration**
- Siera: Scrape stream location data
- Brooke: Scrape tree data
- Upload all cleaned data to repository
- Upload all cleaned data to railway
- ERD
- Document process in data summary as rubric specifies

**Risks and impediments**
- We are at risk of running out of time to complete the data summary, EDA, and feature engineering all this week. We likely will need to move feature engineering to Week 8 where we complete the models. 

## Week 8

**Iteration ending:** <date>
**Milestone tag in focus:** `M2-data-summary`

**Completed PBIs**
- ...

**Stakeholder response log**
- ...

**Plan for next iteration**
- ...

**Risks and impediments**
- ...

**Retrospective (milestone boundary)**
- What worked: ...
- What did not: ...
- One change for next iteration: ...

## Week 9

**Iteration ending:** <date>
**Milestone tag in focus:** `M3-poster-draft`

**Completed PBIs**
- ...

**Stakeholder response log**
- ...

**Plan for next iteration**
- ...

**Risks and impediments**
- ...

## Week 10 -- Poster rough-draft milestone (M3)

**Iteration ending:** <date>
**Milestone tag in focus:** `M3-poster-draft`

**Completed PBIs**
- ...

**Stakeholder response log**
- ...

**Plan for next iteration**
- ...

**Risks and impediments**
- ...

**Retrospective (milestone boundary)**
- What worked: ...
- What did not: ...
- One change for next iteration: ...

## Week 11

**Iteration ending:** <date>
**Milestone tag in focus:** `M4-writeup-draft`

**Completed PBIs**
- ...

**Stakeholder response log**
- ...

**Plan for next iteration**
- ...

**Risks and impediments**
- ...

## Week 12 -- Write-up rough-draft milestone (M4)

**Iteration ending:** <date>
**Milestone tag in focus:** `M4-writeup-draft`

**Completed PBIs**
- ...

**Stakeholder response log**
- ...

**Plan for next iteration**
- ...

**Risks and impediments**
- ...

**Retrospective (milestone boundary)**
- What worked: ...
- What did not: ...
- One change for next iteration: ...

## Week 13

**Iteration ending:** <date>
**Milestone tag in focus:** `M5-final`

**Completed PBIs**
- ...

**Stakeholder response log**
- ...

**Plan for next iteration**
- ...

**Risks and impediments**
- ...

## Week 14 -- Final write-up and poster (M5)

**Iteration ending:** <date>
**Milestone tag in focus:** `M5-final`

**Completed PBIs**
- ...

**Stakeholder response log**
- ...

**Final retrospective**
- What worked: ...
- What did not: ...
- What we would change if we ran this project again: ...

---

## Iteration Review template (copy for any extra week)

```markdown
## Week <NN>

**Iteration ending:** <date>
**Milestone tag in focus:** <M1-proposal | M2-data-summary | M3-poster-draft | M4-writeup-draft | M5-final | infra | ethics>

**Completed PBIs**
- ...

**In-flight (carrying across the boundary)**
- ...

**Stakeholder response log**
- Studio Brief from <peer PO>: adopted = ..., deferred = ..., declined (with reason) = ...

**Plan for next iteration**
- Top PBIs (with milestone tags): ...

**Risks and impediments**
- ...
```
