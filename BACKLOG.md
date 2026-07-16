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
- **GitHub issue:** https://github.com/Serenna4/Emerald-Ash-Borer-Capstone-Project/issues/35 (somehow this one got deleted, re-listed it)

### PBI-002

- **Title:** Draft research question and frame as a testable claim
- **Hypothesis:** We can state the project's research question in one sentence that names the population, the predictor or treatment, and the outcome.
- **Create:** RQ statement in `CHARTER.md` Mission section; one-paragraph framing in the proposal draft.
- **Observe:** can a peer PO who has never seen the project repeat the question back accurately?
- **Analyze:** revise based on Studio Brief feedback.
- **Tag:** `M1-proposal`
- **Size:** Flower
- **GitHub issue:** https://github.com/Serenna4/Emerald-Ash-Borer-Capstone-Project/issues/2 

### PBI-003

- **Title:** Finish Charter Document Touchups
- **Hypothesis:** Review the Charter document once more on Saturday to finalize it.
- **Create:** Review document.
- **Observe:** Ensure no fields are empty.
- **Analyze:** None really. Just refer back to the document to stay on track. 
- **Tag:** M1-proposal
- **Size:** Seed
- **GitHub issue:** https://github.com/Serenna4/Emerald-Ash-Borer-Capstone-Project/issues/3

### PBI-004

- **Title:** Assign Directions for Each of Us
- **Hypothesis:** directions are clear, attainable, and defined. (e.g. Brooke predicting water temperature increase with Ash trees gone)
- **Create:** outlined research questions for each project owner in the project proposal write-up.
- **Observe:** what data we have will determine project directions
- **Analyze:** decide whether each direction is attainable and of equal weight, document in the next Iteration Review.
- **Tag:** M1-proposal
- **Size:** Seed
- **GitHub issue:** https://github.com/Serenna4/Emerald-Ash-Borer-Capstone-Project/issues/4

### PBI-005

- **Title:** Create Data Engineering Plan
- **Hypothesis:**  We can state how the data will be ingested, stored, versioned, and documented.
- **Create:** RQ statement in CHARTER.md Mission section; one-paragraph framing in the proposal draft.
- **Observe:** Can a peer PO who has little knowledge of our data be able to follow our schema and tell how processed data is separated?
- **Analyze:** Revise based on Studio Brief feedback.
- **Tag:** M1-proposal
- **Size:** Forest
- **GitHub issue:** https://github.com/Serenna4/Emerald-Ash-Borer-Capstone-Project/issues/5

### PBI-006

- **Title:** Reach out to Meredith
- **Hypothesis:** We can send Meredith an email and hear back within a reasonable amount of time.
- **Create:** An email to Meredith asking about what would be a good timeline to look at prediciting stream temperature and tree loss in Salem for budgeting and planning.
- **Observe:** What is the best timeline we should use for our project? 2 years? 5 years? 10 years?
- **Analyze:** Decide what timeline to use.
- **Tag:** M1-proposal
- **Size:** Seed
- **GitHub issue:** https://github.com/Serenna4/Emerald-Ash-Borer-Capstone-Project/issues/6

### PBI-007

- **Title:** Collect Data
- **Hypothesis:** We can dowload the data either directly or with an API to have usable data for our project.
- **Create:** Finished uploaded raw data in our repo that is sorted to only include the data we will use in our project.
- **Observe:** We can ensure that the datasets are populated:
- **Analyze:** We ensure there are no apparent discrepancies.
- **Tag:** M2-data summary
- **Size:** Tree
- **GitHub issue:** https://github.com/Serenna4/Emerald-Ash-Borer-Capstone-Project/issues/7

### PBI-008

- **Title:** Select Which Datasets to Use
- **Hypothesis:** We can select some of the datasets to use, based on feedback from Professor Cordova and our Peer POs to narrow down to 3 or 4 datasets.
- **Create:** Sourcing the aforementioned datasets
- **Observe:** Each of these in depth and begin to whittle down our options
- **Analyze:** Final selections with Peer POs and Professor Cordova to confirm and move forward.
- **Tag:** M2-data summary
- **Size:** Flower
- **GitHub issue:** https://github.com/Serenna4/Emerald-Ash-Borer-Capstone-Project/issues/8

### PBI-009

- **Title:** Data Cleaning
- **Hypothesis:** We can go through all of the datasets to ensure that they are aligned to the same level of observation, and that there are no remaining missing values.
- **Create:** Remedying missingness and levels of observation ensuring there is no duplication
- **Observe:** The newly cleaned dataset to ensure that there is no other notable errors across them.
- **Analyze:** Conferring with the Peer POs about patterns of missingness to ensure that the remedying is intuitive.
- **Tag:** M2-data summary
- **Size:** Forest
- **GitHub issue:** https://github.com/Serenna4/Emerald-Ash-Borer-Capstone-Project/issues/9

### PBI-010

- **Title:** Exploratory Data Analysis
- **Hypothesis:** We can start exploring the data by gathering a better understanding of the format of the data. We will gather descriptive statistics which might be included on the Dashboard or for our own background knowledge. We could also start feature engineering to better support our goals of machine learning and prediction.
- **Create:** Summaries of the data and create engineered features for models to use.
- **Observe:** Review summary statistics and use this to remove any needed outliers. Review any engineered features to ensure their values make sense and support our goals
- **Analyze:** Check in with Peer POs and ensure our findings support our mission and make sense to an outside audience. Especially check that any engineered features are sensible.
- **Tag:** M3-Poster rough draft
- **Size:** Tree
- **Github Issue:** https://github.com/Serenna4/Emerald-Ash-Borer-Capstone-Project/issues/10

### PBI-011

- **Title:** Machine learning model for stream temperature for each year (RQ1)
- **Hypothesis:** We will create a model to predict the stream temperature within a given year. Only for 2020, 2022, and 2024.
- **Create:** Regression models have been produced
- **Observe:** Checking that the model make sense to the validation tests (RMSE, MAE, R^2, Cross validation)
- **Analyze:** Peer POs have checked the code and approved it, without displaying obvious logic gaps.
- **Tag:** M3-Poster rough draft
- **Size:** Forest
- **Github Issue:** https://github.com/Serenna4/Emerald-Ash-Borer-Capstone-Project/issues/11

### PBI-012

- **Title:** Machine learning model for predicting stream temps using historical data and weather data (RQ2):
- **Hypothesis:** We will create a model for predicting the stream temperature, adding weather data from 2020, 2022, and 2024.
- **Create:** Try many different regression models to try and accurately predict stream temperature.
- **Observe:** We will observe how each model performs and select the model with the best combination of simplicity, R^2, RMSE, and MAE.
- **Analyze:** Use the performance indicators (RMSE, MAE) to select the best model and look at the trends in the predictions. We will sanity check this work with our Peer POs to ensure the results make sense.
- **Tag:** M3-Poster rough draft
- **Size:** Forest
- **Github Issue:** https://github.com/Serenna4/Emerald-Ash-Borer-Capstone-Project/issues/12

### PBI-013

- **Title:** Regression model for stream temp using canopy coverage (RQ3):
- **Hypothesis:** We will create a regression model for predicting the stream temp using historical data and canopy cover data in 2020, 2022, and 2024.
- **Create:** A regression model that measures the stream temp for each year.
- **Observe:** Do our model’s validation tests (R^2, RMSE, MAE, and cross-validation) make sense to our peers?
- **Analyze:** Do our model’s validation tests (R^2, RMSE, MAE, and cross-validation) make sense to other peers not in our natural resources group?
- **Tag:** M3-Poster rough draft
- **Size:** Forest
- **Github Issue:** https://github.com/Serenna4/Emerald-Ash-Borer-Capstone-Project/issues/13

### PBI-014

- **Title:** Create Exploratory Data Analysis Visualizations
- **Hypothesis:** We can create 2 graphs to showcase the trends in the data and the impact of rising stream temps.
- **Create:** One graph showing the stream temp change by season from 2016 to 2024. And another graph showing the relationship between stream temperature and dissolved oxygen in streams.
- **Observe:** We will observe the graphs and perform and polishing to get them publish ready.
- **Analyze:** These graphs will help tell the story of our project and its impact. We will ask our Peer POs to review these graphs and ensure they support our message as we intend.
- **Tag:** M3-Poster rough draft
- **Size:** Tree
- **Github Issue:** https://github.com/Serenna4/Emerald-Ash-Borer-Capstone-Project/issues/14

### PBI-015

- **Title:** Create Model Graphics
- **Hypothesis:** We can create graphics regarding our models to demonstrate how we picked the best model and what values were most important to it.
- **Create:** We can create graphs for each research question showing which model performed the best using our evaluation metrics. We can also create a graph showing the primary variables being used in the models for the highest performing models.
- **Observe:** We will make sure these graphs are publish ready and support our story.
- **Analyze:** We will ask our Peer POs to give us feedback on the graphs for a sanity check and to make sure they work well with the rest of our material
- **Tag:** M3-Poster rough draft
- **Size:** Tree
- **Github Issue:** https://github.com/Serenna4/Emerald-Ash-Borer-Capstone-Project/issues/15

### PBI-016

- **Title:** Add Data We Have to Repo (Small Part of Collect Data Task)
- **Hypothesis:** Broken up part of collecting data. We have some data, add it to the repository.
- **Create:** Finished downloaded and uploaded raw data in our repo that we already have linked.
- **Observe:** We can successfully download the data sources we have.
- **Analyze:** We ensure there are no apparent discrepancies in our current sources.
- **Tag:** M2-data summary
- **Size:** Flower
- **GitHub issue:** https://github.com/Serenna4/Emerald-Ash-Borer-Capstone-Project/issues/16

### PBI-017

- **Title:** Scrape Shapefile for Streams
- **Hypothesis:** We can create a custom shapefile from a map of the streams included in the stream data we received from the city of Salem
- **Create:** A shapefile of the stream locations to be used in predicting tree risk, prevalence, and stream temp.
- **Observe:** row counts, missingness, key uniqueness. Ensure that we can combine it with stream temp data.
- **Analyze:** decide whether the dataset survives feasibility; document in the next Iteration Review.
- **Size:** Tree
- **Github issue:** https://github.com/Serenna4/Emerald-Ash-Borer-Capstone-Project/issues/17

### PBI-018

- **Title**: Brooke: Scrape Tree Data
- **Hypothesis:** We can scrape the data for trees in Salem from the website with Cordova. Receive template from Cordova for tree scraping at the weekly level. Acquire and clean the data.
- **Create:** A CSV of tree locations in Salem.
- **Observe:** Row counts, missing ness, key uniqueness. Ensure that the data is accurate.
- **Analyze:** Decide whether the dataset survives the feasibility.
- **Size:** Tree
- **Github Issue:** Github Issue: https://github.com/Serenna4/Emerald-Ash-Borer-Capstone-Project/issues/18

### PBI-019

- **Title:** Serenna: Clean EAB data
- **Hypothesis:** We can scrape the EAB data from the website with Cordova. Receive template from Cordova for EAB scraping. Remove false identifications from the dataset.
- **Creates:** A CSV of the EAB sightings in Salem.
- **Observe:** Row counts, missingness, key uniqueness. Ensure that the data is accurate.
- **Analyze:** Decide whether the dataset survives the feasibility. 
- **Size:** Tree
- **Github Issue:** https://github.com/Serenna4/Emerald-Ash-Borer-Capstone-Project/issues/19

### PBI-020

- **Title:** Siera: Cleaning Stream Temperatures
- **Hypothesis:** We can aggregate stream temperatures to the weekly level.
- **Creates:** A CSV of the stream temperatures in Salem.
- **Observe:** Row counts, missing ness, key uniqueness. Ensure that the data is accurate.
- **Analyze:** Decide whether the dataset survives the feasibility. 
- **Size:** Tree
- **Github Issue:** https://github.com/Serenna4/Emerald-Ash-Borer-Capstone-Project/issues/20

### PBI-021

- **Title:** Brooke: Clean Temperature Data
- **Hypothesis:** We can aggregate weather temperatures to the month level. Select weather station and relevant weather columns.
- **Creates:** A CSV of the EAB sightings in Salem.
- **Observe:** Row counts, missing ness, key uniqueness. Ensure that the data is accurate.
- **Analyze:** Decide whether the dataset survives the feasibility. 
- **Size:** Tree
- **Github Issue:** https://github.com/Serenna4/Emerald-Ash-Borer-Capstone-Project/issues/23

### PBI-022

- **Title:** Select Best Datasets
- **Hypothesis:** We can select a subset of our datasets to accommodate our research question.
- **Create:** Download all datasets necessary, about 3-5.
- **Observe:** We can successfully read (human) all of the datasets after the download.
- **Analyze:** We can ensure all of our research question needs are covered by the selected data.
- **Tag:** M2-data summary
- **Size:** Flower
- **Github issue:** https://github.com/Serenna4/Emerald-Ash-Borer-Capstone-Project/issues/24

### PBI-023

- **Title:** Collect zip-code density data
- **Hypothesis:** If I can gather information on the population density by zip-code, this could be an important feature to use in our models.
- **Create:** Scrape or download a dataset on zip-code density data
- **Observe:** Review the data to ensure it aligns with our purpose.
- **Analyze:** Perform any necessary data cleaning and move the data into our github and railway account.
- **Tag:** M2-Data Summary
- **Size:** Tree
- **Github Issue:** https://github.com/Serenna4/Emerald-Ash-Borer-Capstone-Project/issues/25

### PBI-024

- **Title:** Regression Model for stream temps using weather and canopy coverage (RQ#4)
- **Hypothesis:** We can create a regresison model that uses historical stream data, weather data, and canopy coverage data to make the model even more accurate.
- **Create:** Multiple regression models for each year in 2020, 2022, and 2024.
- **Observe:** We will evaluate this model using RMSE, MAE, cross validation, and R^2.
- **Analyze:** We will use our metrics to determine if the model is better or worse than the previous ones. We will check in with our Peer POs to do a sanity check on the results.
- **Tag:** M3-Poster rough draft
- **Size:** Forest
- **Github Issue:** https://github.com/Serenna4/Emerald-Ash-Borer-Capstone-Project/issues/27

### PBI-025

- **Title:** Create Poster Rough Draft
- **Hypothesis:** We can create a first draft of our poster using the template provided by Prof. Cordova.
- **Create:** We can fill in every setion with either the appropriate text/visualizations or we can fill in the sections with the anticipated information if analysis is not completed.
- **Observe:** We will evaluate the format, context, and organization of the poster to determine what we want to change for the final draft.
- **Analyze:** We will have our Peer POs evaluate the poster draft and incorporate any feedback into our final draft plans.
- **Tag:** M3-Poster rough draft
- **Size:** Forest
- **Github Issue:** https://github.com/Serenna4/Emerald-Ash-Borer-Capstone-Project/issues/28

### PBI-026

- **Title:** Write-up First Draft
- **Hypothesis:** We can create a first-draft of our write up summarizing our methods and findings.
- **Create:** We will create a rough draft of the write up for feedback.
- **Observe:** We will review the document to find areas for improvement for the final version
- **Analyze:** We will ask our Peer POs to review the document to suggest any improvements for the final version
- **Tag:** M4-Write-up Draft
- **Size:** Forest
- **Github Issue:** https://github.com/Serenna4/Emerald-Ash-Borer-Capstone-Project/issues/29

### PBI-027

- **Title:** Create Final Poster Iteration
- **Hypothesis:** We can use previous feedback to improve and polish our final version of the poster.
- **Create:** Add and modify any sections of the poster that need it.
- **Observe:** Make sure the poster is polished and presentation-ready. Ensure text is readable
- **Analyze:** Make sure the story flows on the poster and is easy to understand and follow.
- **Tag:** M5-Final Submission
- **Size:** Tree
- **Github Issue:** https://github.com/Serenna4/Emerald-Ash-Borer-Capstone-Project/issues/30

### PBI-028

- **Title:** Create Final Write-Up Iteration
- **Hypothesis:** We can use previous feedback to improve and polish our final version of the write-up.
- **Create:** Add and modify any sections of the write-up that need it. Save the final version in Github
- **Observe:** Make sure the write-up is polished and accurate.
- **Analyze:** Have others peer-edit our write-up to ensure it is easy to understand and follow.
- **Tag:** M5-Final Submission
- **Size:** Tree
- **Github Issue:** https://github.com/Serenna4/Emerald-Ash-Borer-Capstone-Project/issues/31

### PBI-029

- **Title:** Github Touch Ups
- **Hypothesis:** We will fill in any overlooked areas of documentation in the Github
- **Create:** We will review the entire Github project and ensure all documentation is filled out and necessary files are included.
- **Observe:** We will explore the github to find any areas missing information.
- **Analyze:** N/A
- **Tag:** M5-Final Submission
- **Size:** Tree
- **Github Issue:**  https://github.com/Serenna4/Emerald-Ash-Borer-Capstone-Project/issues/32

### PBI-030

- **Title:** Amend Project Proposal
- **Hypothesis:** We have changed the trajectory of our project so we should write another project proposal for consistency.
- **Create:** We will create a new project proposal that amends the original one to align with our new project direction.
- **Observe:** We will ensure the new adjustments align with our new project goals to keep us on track and for clarity in the future.
- **Analyze:** We will have peer POs review the project proposal to bring up any other concerns.
- **Tag:** M1-Project proposal
- **Size:** Tree
- **Github Issue:** https://github.com/Serenna4/Emerald-Ash-Borer-Capstone-Project/issues/33

### PBI-031

- **Title:** Amend Data Summary
- **Hypothesis:** After adjusting our project proposal, we want to adjust the data summary since our data sources have also changed in our pivot.
- **Create:** Edit the data summary to reflect new changes in our project trajectory
- **Observe:** Ensure the new data summary is accurate and sets us up for success by organizing how all data connects and related to each other.
- **Analyze:** Have peer POs and our experts review the new plan and data summary to bring up any new concerns early.
- **Tag:** M2-Data summary
- **Size:** Flower
- **Github Issue:** https://github.com/Serenna4/Emerald-Ash-Borer-Capstone-Project/issues/34

### PBI-032

### PBI-033

### PBI-034

### PBI-035
