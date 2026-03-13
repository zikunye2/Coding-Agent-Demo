# Coding Agent Demo

Two hands-on demos using coding agents (Claude Code, Cursor, Copilot, etc.).

## Setup

1. Clone this repo: `git clone https://github.com/zikunye2/Coding-Agent-Demo.git`
2. Open your coding agent in the cloned folder

---

## Demo 1: Data Analysis

Build a customer churn prediction pipeline from raw data to a business report.

**Working folder**: `data-analysis/`

### Step 1 — Explore the data

```
Install the dependencies in requirements.txt, then load telco_churn.csv and
do exploratory data analysis. Show me the shape of the data, missing values,
churn distribution, and a few visualizations. Save all figures to a figures/ folder.
```

### Step 2 — Train a model

```
Preprocess the data (handle any data type issues, encode categoricals,
train/test split, standardize features). Train an XGBoost classifier with
GridSearchCV hyperparameter tuning (small grid for speed, 3-fold CV).
Show me accuracy, AUC-ROC, precision, recall, F1. Save confusion matrix,
ROC curve, and feature importance plot to figures/.
```

### Step 3 — Write a business report

```
Write a report.md summarizing the full analysis. Include:
- Executive summary with key metrics
- Embedded figures using relative paths to figures/
- Top 10 feature importance with business interpretation
- 3 actionable retention strategy recommendations
Make it professional and presentation-ready.
```

---

## Demo 2: Personal Website

Turn a resume into a live portfolio website.

**Working folder**: `personal-website/`

### Before you start

Open `inputs/sample_resume.md` and replace it with your own info (or keep the sample).

### Step 1 — Build the site

```
Read my resume from inputs/sample_resume.md and the project summary from
inputs/project1_summary.md. Update website/devportfolio-master/src/config.ts
with my information: name, title, about me, skills, experience, education,
and projects. Keep it accurate — don't add anything not in the source files.
```

### Step 2 — Preview

```
Install dependencies and start the dev server so I can see the site.
```
