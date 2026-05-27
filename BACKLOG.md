# Backlog: <project name>

This file is the **human-readable mirror** of the [GitHub Projects (v2) Iterative Development board](https://docs.github.com/en/issues/planning-and-tracking-with-projects/learning-about-projects/about-projects) for this repo. Every row here is also a GitHub issue, added to the board, tagged with a milestone label, and sized.

## Conventions

- Each item has: id, title, hypothesis or user story, **Create / Observe / Analyze** triple, milestone tag, size.
- Items are ordered top to bottom by **priority**.
- Milestone tags: `M1-proposal`, `M2-data-summary`, `M3-poster-draft`, `M4-writeup-draft`, `M5-final`, `infra`, `ethics`.
- Sizes: S, M, L, XL.
- The board has five columns: `Backlog` → `Create` → `Observe` → `Analyze` → `Done`. Each column is the *phase of work happening on a single PBI right now*, not a work type. See the [Iterative Development board explainer](https://courses.lpcordova.phd/data510/project-framework/#github-projects-board-per-project-iterative-development-board) for what each column means and when to advance a card.
- WIP cap: `Create + Observe + Analyze` ≤ `owners + 1` at any time.
- Definition of Ready and Definition of Done live in [`CHARTER.md`](CHARTER.md).

## Items

### PBI-001

- **Title:** Acquire and document <dataset>
- **Hypothesis:** <dataset> is accessible, license-compatible, and large enough to answer <RQ>.
- **Create:** ingestion script and `data/README.md` section describing schema.
- **Observe:** row counts, missingness, key uniqueness, distribution sanity checks.
- **Analyze:** decide whether the dataset survives feasibility; document in the next Iteration Review.
- **Tag:** `M1-proposal`
- **Size:** Flower
- **GitHub issue:** <link once filed>

### PBI-002

- **Title:** Draft research question and frame as a testable claim
- **Hypothesis:** We can state the project's research question in one sentence that names the population, the predictor or treatment, and the outcome.
- **Create:** RQ statement in `CHARTER.md` Mission section; one-paragraph framing in the proposal draft.
- **Observe:** can a peer PO who has never seen the project repeat the question back accurately?
- **Analyze:** revise based on Studio Brief feedback.
- **Tag:** `M1-proposal`
- **Size:** S
- **GitHub issue:** <link once filed>

### PBI-003

- **Title:** Finish Charter Document Touchups
- **Hypothesis:** Review the Charter document once more on Saturday to finalize it.
- **Create:** Review document.
- **Observe:** Ensure no fields are empty.
- **Analyze:** None really. Just refer back to the document to stay on track. 
- **Tag:** M1-proposal
- **Size:** Seed
- **GitHub issue:** 

### PBI-004

- **Title:** Assign Directions for Each of Us
- **Hypothesis:** directions are clear, attainable, and defined. (e.g. Brooke predicting water temperature increase with Ash trees gone)
- **Create:** outlined research questions for each project owner in the project proposal write-up.
- **Observe:** what data we have will determine project directions
- **Analyze:** decide whether each direction is attainable and of equal weight, document in the next Iteration Review.
- **Tag:** M1-proposal
- **Size:** Seed
- **GitHub issue:**

### PBI-005

- **Title:** Create Data Engineering Plan
- **Hypothesis:**  We can state how the data will be ingested, stored, versioned, and documented.
- **Create:** RQ statement in CHARTER.md Mission section; one-paragraph framing in the proposal draft.
- **Observe:** Can a peer PO who has little knowledge of our data be able to follow our schema and tell how processed data is separated?
- **Analyze:** Revise based on Studio Brief feedback.
- **Tag:** M1-proposal
- **Size:** Forest
- **GitHub issue:**

