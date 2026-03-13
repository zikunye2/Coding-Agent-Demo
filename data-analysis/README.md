# Demo 1: Data Analysis with a Coding Agent

## Overview

Use a coding agent to build a complete customer churn prediction pipeline — from data exploration to a final business report with figures — in one prompt.

**Dataset**: Telco Customer Churn (~7,000 customers, 21 features)
**Task**: Predict which customers will churn (binary classification)
**Model**: XGBoost with GridSearchCV hyperparameter tuning
**Output**: `report.md` + `figures/` directory — a complete, presentation-ready report

## Files

| File | Description |
|------|-------------|
| `telco_churn.csv` | Telco customer churn dataset |
| `requirements.txt` | Python dependencies |
| `completed/` | Reference output: script, report, and all figures |

## Quick Start

1. Open any coding agent (Claude Code, Cursor, Copilot, Gemini CLI, etc.)
2. Navigate to this folder
3. Paste the prompt below

## Prompt

```
You are working in the data-analysis/ folder.

Dataset: telco_churn.csv — Telco Customer Churn dataset (~7000 customers).
Target variable: Churn (Yes/No).

Task: Write a Python script (churn_analysis.py) that performs a complete
analysis and generates a final business report. The script should:

1. Load and explore the data (save EDA visualizations to figures/)
2. Preprocess: fix TotalCharges, encode categoricals, train/test split,
   standardize features
3. Train XGBoost with GridSearchCV hyperparameter tuning (keep the grid
   small for speed, e.g. 2 values per param, 3-fold CV) — save tuning
   heatmap, feature importance plot, confusion matrix, and ROC curve
4. Evaluate the model: accuracy, AUC-ROC, precision, recall, F1-score
5. Generate report.md — a professional business report with:
   - Executive summary with key metrics
   - Embedded figures (using relative paths to figures/)
   - Hyperparameter tuning results table
   - Top 10 feature importance with business interpretation
   - 3 actionable retention strategy recommendations

After writing the script, run it to generate all outputs.
Dependencies are in requirements.txt — install them first.
```
