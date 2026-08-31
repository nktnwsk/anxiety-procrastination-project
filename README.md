# Procrastination Patterns in University Students: The Role of Gender & Anxiety Diagnosis

This repository contains the full R data processing pipeline, psychometric reliability calculations, and visualisation scripts for an empirical study examining how worry-related anxiety symptoms relate to task procrastination among university students.

> **Research Question:** Can higher levels of worry-related anxiety symptoms be associated with greater levels of behavioral procrastination?

---

## Key Highlights & Findings

* **Sample:** $N = 56$ adults (aged 18–30)
* **Primary Result:** A statistically significant, moderate positive correlation between anxiety symptoms (PSWQ) and procrastination (Lay's Scale), $r(54) = .37, p = .005$.
* **Demographics:** Sample divided by self-reported **gender** and **history of clinical anxiety diagnosis** to evaluate additional potential patterns.

---

## Measures & Method

1. **Penn State Worry Questionnaire (PSWQ):** 16 items measuring uncontrollable worry.
2. **Lay's Procrastination Scale:** 20 items measuring behavioural task delay.

### Analytical Pipeline (R)
* Reverse scoring for Likert-type scales ($6 - X$).
* Cronbach’s $\alpha$ internal consistency evaluation.
* Pearson’s $r$ correlation testing.
* Non-parametric LOESS curve estimation for subgroup visualizations.

---

## Repository Structure

```text
├── anxiety-procrastination.Rproj     # RStudio Project file
├── data/
│   └── APP.csv                       # Raw anonymised survey responses
├── data-analysis-code.Rmd            # R Markdown pipeline & report
├── index.html                        # Live rendered report
├── README.md                         # General repository documentation
└── Research_Paper.pdf                # The original paper
```

---

## Author's Note on software usage:
Originally, statistical analyses, tables, and figures, presented in the paper (.pdf), were generated in jamovi. Since jamovi runs on R, the .Rmd pipeline in this repository is set to reproduce identical statistical calculations directly in the native R (ggplot2, dplyr, knitr, etc). Visually, the style varies between jamovi outputs and the standard R render, yet all mathematical results remain correct and identical. 