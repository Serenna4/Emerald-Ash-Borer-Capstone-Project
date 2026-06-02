# Studio Charter: Protecting Salem’s Ecosystem by Preventing the Spread of the Emerald Ash Borer

> Filled in live during the **Studio Charter** session in week 3. Every section below is committed in the same commit at the end of that class block. See [Studio Charter (single-session inception)](https://courses.lpcordova.phd/data510/project-framework/charter-inception.html) for the script and time-boxes.

- **Owner team:** Siera Edwards, Serenna Walter, and Brooke Proctor
- **Owner Product Lead:** Serenna Walter
- **Peer Stakeholder POs:** Amaya Supancich-McCord, Spencer Fiden
- **Instructor / Sponsor:** Lucas Cordova (`LucasCordova` on GitHub)
- **GitHub repo:** https://github.com/Serenna4/Emerald-Ash-Borer-Capstone-Project
- **GitHub Projects board:** https://github.com/users/Serenna4/projects/2
- **Discord category:** `#Project 21`
- **Studio Session:** 3
- **Studio formed:** 5/25/2026

## Vision

Our project aims to add to the current knowledge within the Forestry, Conservation, Ecology, and Environmental Science realms. We were given data and some project inspiration by Meridith Greer from the City of Salem Department of Natural Resources so our goal is to contribute to their knowledge to further prevent the spread of the Emerald Ash Borer. 

## Mission

We want to create an interactive map and a dashboard to show the areas most at risk of the infestions of the Emerald Ash Borer and recommend ways to prevent the spread. 
Research questions:
- Can we predict which stands of trees Emerald Ash Borers are likely to infest in Salem?
- Can we model what riparian zones along Salem’s waterways will look like in the next 5 years?
- Can we predict how stream temperatures will be affected by a loss of Oregon Ash trees?


## Context

- **Users / affected parties:**
    - Local communitieis and the environment are affected and benefited by this project.
    - At risk are ash trees (primarily in Oregon), white fringe trees, and olive trees. 
- **Data sources (proposed):** named sources, access status, license / ethics notes.
    - Emerald Ash Borer (EAB) in Oregon: https://oregon-eab-geo.hub.arcgis.com/
        - Access: Publically accessible online map. We are unsure of how to download the data itself. 
        - Ethics: It might not be a representative survey. This is data from the state, which is reliable, but it could be more influenced to locations that are around public areas.
    - Willamette Valley Hardwoods Model Vector Tile Layer: https://geo.maps.arcgis.com/home/item.html?id=b48f922706014b63b18a56734d647e2b
        - Access: Publically accessible online map. We are unsure of how to download the data itself. 
        - Ethics: It might not be a representative survey. This is data from the state, which is reliable, but it could be more influenced to locations that are around public areas.
    - TreePlotter: https://pg-cloud.com/Oregon/
        - Access: Publically accessible online map. We are unsure of how to download the data itself. 
        - Ethics: It might not be a representative survey. This is data from the state, which is reliable, but it could be more influenced to locations that are around public areas.
    - Oregon EAB Trap App: https://geo.maps.arcgis.com/apps/mapviewer/index.html?webmap=cd7f5da6130749a9b7b99a45844b0f24
        - Access: Publically accessible online map. We are unsure of how to download the data itself. 
        - Ethics: It might not be a representative survey. This is data from the state, which is reliable, but it could be more influenced to locations that are around public areas.
    - Waterway Locations
        - Access: Not achieved yet
    - Temperature and Humidity
        - Access: Not achieved yet
    - Population Density (mostly transported by people moving wood)
        - Access: Not achieved yet
    - Type of Area (Rural vs. Urban)
- **Constraints:** time, compute, access, skills, scope.
    - Time: We want to have data over time. We want to predict for next year. 
    - Scope: We will have to pick a difinitive area to look at.
    - Access: Downloading data from publically accessible map.
    - Skills: Bringing GIS data into postgres.
- **Ethics risks:** consent, retention, PII, fairness, deployment risk.
    - Data Accessibility: We aren't anticipating issues with open data.
    - Deployment risks: We are a bit worried that our predictions could be inaccurate and could put up preventative measures in the wrong areas.

## Success criteria by milestone

- **M1, proposal (W4):**
    - We have a strong start on the datasets that we want to include in our project and their accessiblity status.
    - We have a strong plan for the upcoming weeks and a clear direction of how we need to move forward.
    - We have risks and current areas of uncertainty listed in our project as well as ways to combat them.
- **M2, data summary (W7):**
    - We know what data is viable and have sorted out the data that is not accessible or relevant.
    - We have enough data to answer our research questions. 
- **M3, poster rough draft (W10):**
    - Our visualizations are 80% of what we expect to have on the final draft so that we can get effective feedback.
    - We have visualizations that begin to show how we analyzed our research questions.
    - We have a plan for how we want to edit our visualizations in the future.
- **M4, write-up rough draft (W12):**
    - The rough draft includes clear analysis that backsup the answers of our research questions.
    - The rough draft is at least 80% of what we expect our final draft to be.
- **M5, final write-up and poster (W14):**
    - People are able to use our dashboard and interactive map to determine what areas in Salem are high-risk and get ideas on how to protect these areas.
    - People are able to use our dashboard and interactive map to see what the impact would be on Salem's stream temperatures and broader environment if infestations continued as they have historically. 

## Working agreements (internal to owner team)

- **Sync rhythm:** We are meeting at 11am most Saturdays.
- **Code review:** At each meeting, we will assign tasks for each of us to do. We will check in and review with each of our code at each meetings.
- **Decision rule:** If special circumstances come up, we will text about it and decide together.

## Working agreements (triad with peer POs)

- **Studio Brief due:** by 5 pm the Sunday before class, committed to `studio/briefs/W<NN>-<peer>.md` and linked in our Google Chat. 
- **Studio Critique due:** by Midnight the Wednesday after class.
- **Swim Lanes due:** by 5pm the Saturday after class
- **Priority conflict resolution:** owner team integrates briefs in good faith; the instructor arbitrates (as Process Expert) if peer POs and owner team disagree.

## Response SLAs (Service Level Agreements)

A **Service Level Agreement** is a written promise the triad makes about *how fast* each side responds when a specific signal arrives. Every row must have an answer before this Charter is committed. See [Response SLAs](https://courses.lpcordova.phd/data510/project-framework/charter-inception.html#response-slas-service-level-agreements) for the full definition.

| When this signal arrives... | Who responds | By when |
|-----------------------------|--------------|---------|
| Peer PO files a **Studio Brief** (commits to `studio/briefs/...`, links in Google Chat) | Owner team | Acknowledge in Google Chat by Monday at 6pm, with a first-pass adopt / defer / decline call for each item |
| Peer PO files a **Studio Critique** | Owner team | Respond in Google Chat by Saturday at 5pm and capture follow-up items into the backlog |
| Owner team posts an **Iteration Review** in `README.md` | Both peer POs | Read before filing the next Brief and Critique. |
| Owner team flags a **blocker** in our Google Chat | Instructor, plus any tagged peer PO | Responds by the next Studio Session at the latest; faster if online. Send a text if you want feedback. |
| Anyone asks a clarifying question in our Google Chat | Whoever is tagged (default: owner team) | Reply within 48 hours, even if the reply is "we will look at this next iteration". Send a text in the chat. |

## Definition of Ready (PBI)

A PBI is ready to be pulled out of `Backlog` and moved into `Create` when it has:

- A one-sentence hypothesis or user story.
- A named **Create**, **Observe**, **Analyze** triple.
- A milestone tag (`M1-proposal`, `M2-data-summary`, `M3-poster-draft`, `M4-writeup-draft`, `M5-final`, `infra`, `ethics`).
- A T-shirt size estimate (Seed, Flower, Tree, Forest).
- WIP slack on the board: `Create + Observe + Analyze` is below the team's WIP cap (owners + 1).

## Definition of Done (PBI)

A PBI is done, and may be moved from `Analyze` into `Done`, when:

- The Create artifact is in the repo or linked from the issue.
- The Observe results are recorded somewhere referenceable (notebook output, processed dataset, draft results section).
- The Analyze writeup names a next step (continue, pivot, kill, or decompose into new PBIs).
- A peer PO has either signed off in our Google Chat or filed a Studio Critique covering it.
- The card is linked under *Completed PBIs* in the next Iteration Review in `README.md`.

## Context map

> Optional. Replace this block with a Mermaid `flowchart LR` showing how users, data, constraints, and ethics risks flow into the owner team and out to the capstone outcome. See the [`charter-inception.qmd` template](https://courses.lpcordova.phd/data510/project-framework/charter-inception.html) for a starting Mermaid diagram.

## Stakeholder alignment memo (one-page summary)

### Why we exist
Our project aims to add to the current knowledge within the Forestry, Conservation, Ecology, and Environmental Science realms. We hope that this project could be used by government or private organizations to further prevent the spread of the Emerald Ash Borer. We want to create an interactive map and a dashboard to show the areas most at risk of the infestions of the Emerald Ash Borer and recommend ways to prevent the spread.

### What we will deliver to peer POs every week
- An Iteration Review in this `README.md` by **Saturday / 5pm**
- A summary of which Studio Brief items we adopted, deferred, or declined and why

### What we need from peer POs every week
- A Studio Brief by **Sunday / 5pm** next class (next iteration's requirements, questions, risks)
- A Studio Critique by **Wednesday / 5pm** next class (assessment of last week's delivery)

### How to reach us
- Main Communication: Google Chat
- Discord category: `#Project 21`
- GitHub repo: https://github.com/Serenna4/Emerald-Ash-Borer-Capstone-Project
- GitHub Projects board: https://github.com/users/Serenna4/projects/2
