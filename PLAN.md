# PLAN.md — Project and Repository Plan

---

## Part 1: Project Plan

### Goals

The goal of this project is to conduct a reproducible data analysis using Quarto (QMD) for STAT 184. The analysis will explore three distinct datasets and questions:

1. **Airport Passenger Traffic (2020-2024):** Examine and visualize trends in passenger traffic across six major international airports — ATL (Atlanta), DXB (Dubai), LHR (London Heathrow), DFW (Dallas/Fort Worth), FRA (Frankfurt), and PKX (Beijing Daxing) — over the five-year period from 2020 to 2024.
2. **Pirate Beard Length by College:** Use the {yarrr} R package's built-in pirates dataset to investigate whether beard length varies by the college a pirate attended, using appropriate summary statistics and visualizations.
3. **Monte Carlo Simulation:** Design and run a Monte Carlo simulation using simulated data to demonstrate probabilistic estimation (e.g., estimating pi or expected values), and visualize the convergence or distribution of results.

### Needs

- Access to Wikipedia's "List of Busiest Airports by Passenger Traffic" for airport data (web scraping or manual table entry)
- The {yarrr} R package installed in R for the pirates dataset
- A random number generator / simulation framework in R for the Monte Carlo component
- Quarto installed and configured to render to both HTML and PDF
- R packages: tidyverse, ggplot2, yarrr, knitr, dplyr

### Steps

1. Set up the Quarto (.qmd) document with YAML front matter (title, author, format: pdf)
2. Airport Traffic: Scrape or manually import the Wikipedia airport passenger data table; clean and reshape the data; create a line or bar chart showing traffic trends by airport from 2020-2024
3. Pirate Beards: Load the pirates dataset from {yarrr}; group by college; compute summary statistics (mean, median, SD) for beard length; create a boxplot or violin plot
4. Monte Carlo: Write a simulation function (e.g., random point sampling); run it for increasing iteration counts; plot the running estimate to show convergence
5. Add narrative text, code chunks with appropriate chunk options, and captions to all figures
6. Render the final .qmd to PDF and verify output

---

## Part 2: Repository Plan

### Goals

The goal of this repository plan is to set up and maintain a well-organized GitHub repository for HW 4.4 that follows best practices for version control, issue tracking, and collaborative workflow. The repo demonstrates proficiency with branching, issues, commits, and pull requests as required by STAT 184.

### Needs

- A GitHub repository named Stat184_HW4.4_Nikhil (already created)
- A main branch as the stable, production-ready branch
- A dev branch for all active development and file additions
- GitHub Issues to track each major task with appropriate labels
- Descriptive commit messages following the imperative mood convention
- A pull request to merge dev into main once all work is complete
- A finalized README.md that documents all files in the repository

### Steps

1. Branch: Create a dev branch off main to serve as the working branch for all additions
2. Issues: Open three issues to track the three major tasks:
   - Issue #1: "Add PLAN.md document" (label: documentation)
   - Issue #2: "Add HW 4.3 files (QMD and PDF)" (label: enhancement)
   - Issue #3: "Finalize README" (label: documentation)
3. Commit PLAN.md: Create and commit this PLAN.md file to dev, referencing Closes #1 in the commit body
4. Commit HW 4.3 files: Upload hw43.qmd and hw43.pdf to the dev branch and commit, referencing Closes #2 in the commit body
5. Finalize README: Update README.md on dev to list and describe all files in the repository, then commit referencing Closes #3
6. Pull Request: Open a pull request from dev to main with a descriptive title and summary of changes
7. Merge: Merge the pull request so main reflects the completed, finalized state of the project
8. Verify: Confirm all three issues are closed and main branch contains all expected files
