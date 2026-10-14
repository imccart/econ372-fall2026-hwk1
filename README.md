# Econ 372, Fall 2026: Homework 1 Solutions

This repository is one complete solution to Homework 1, set up the same way the
homework template asked you to set up yours. The point is less the specific
answers than the workflow, so you can see one way to organize a Quarto file and a
repository for an empirical assignment.

## What's in here

- `code/analysis.qmd` is the Quarto source, with a short setup chunk and then one
  section per question. Each part has its code, its output, and a few sentences
  that state the result.
- `code/report.html` is the rendered report. Download it and open it in a browser
  to read the solutions without running anything.
- `nj-ihc.csv` is the New Jersey dataset built for Question 1. It sits outside
  `data/` so that it is included in the repository.
- `data/` holds the two Medicare files for Question 2. Like in the template, git
  ignores this folder, so the raw data is not uploaded.

The commit history shows the order of the work, starting from the template, then
Question 1, then Question 2, then the rendered report.

## Running it yourself

Put `medicare-ma-penetration.csv` and `medicare-ffs-costs.csv` from the course
OneDrive into `data/`, then render from the top of the repository:

```
quarto render code/analysis.qmd
```

The R packages used are tidyverse, scales, and knitr.
