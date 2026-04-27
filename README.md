# Supermarket Sales Analysis & Prediction

> Comprehensive analysis of supermarket sales across 3 branches over 3 months —  
> combining MySQL data cleaning, Python EDA & visualizations, and ML-based  
> sales peak prediction.

![Python](https://img.shields.io/badge/Python-3.10-blue?style=flat-square)
![MySQL](https://img.shields.io/badge/MySQL-Data%20Cleaning-lightblue?style=flat-square)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-Predictive%20Model-orange?style=flat-square)
![Matplotlib](https://img.shields.io/badge/Matplotlib-Visualizations-green?style=flat-square)
![Status](https://img.shields.io/badge/Status-Complete-brightgreen?style=flat-square)

---

## Overview

This project delivers an end-to-end analysis of a supermarket chain's sales data across
three branches. Starting with SQL-based data cleaning, moving through exploratory analysis
and visual storytelling in Python, and culminating in a predictive model for forecasting
peak sales periods — the goal is to surface actionable insights for inventory planning,
staffing, and marketing strategy.

---

## Project Phases

### Phase 1 — Data Cleaning (MySQL)
- Cleaned and structured raw transactional sales data
- Handled nulls, duplicates, and inconsistent formatting
- Created SQL views for targeted analysis perspectives, including
  `time_based_analysis` for time-series work downstream

### Phase 2 — Exploratory Analysis & Visualizations (Python)
All visualizations built with **Matplotlib** and **Seaborn** across four analysis areas:

**Branch performance**
- Revenue and transaction volume by branch (A, B, C)
- Branch efficiency comparisons over the 3-month window

**Product line analysis**
- Top and bottom performing product categories
- Revenue share per product line per branch

**Customer behaviour**
- Purchasing patterns: member vs. non-member customers
- Average basket size and visit frequency by customer type

**Temporal trends**
- Daily, weekly, and monthly sales patterns
- Peak sales day identification across branches
- Time-of-day transaction distribution

### Phase 3 — Predictive Modelling (Python / Scikit-Learn)
- Built on the `time_based_analysis` SQL view as the modelling dataset
- Trained ML models to forecast peak sales dates
- Evaluated using MAE and RMSE across time-series cross-validation splits

> Status: In progress — model training notebook available in `python_scripts/`

---

## Key Insights

| Area | Finding |
|---|---|
| Branch performance | Branch-level variance in revenue and transaction efficiency identified |
| Product trends | Top-performing product lines and customer preferences surfaced |
| Customer behaviour | Clear spending differences between member and non-member segments |
| Temporal patterns | Recurring daily and weekly sales peaks identified across branches |

---

## Repository Structure

```
supermarket-sales/
├── data/                          # Cleaned datasets and exported SQL views
├── sql_scripts/                   # MySQL cleaning scripts and view definitions
├── python_scripts/
│   ├── predictive_model.ipynb     # ML model for peak sales prediction
│   └── models/                    # Saved trained model files
├── docs/                          # Analysis reports and insight summaries
├── requirements.txt               # Python dependencies
└── LICENSE.md
```

---

## How to Run

```bash
# Clone the repo
git clone https://github.com/Toni8/<Supermarket-sales>.git
cd supermarket-sales

# Install dependencies
pip install -r requirements.txt

# Or manually
pip install pandas numpy matplotlib seaborn scikit-learn jupyter
```

**Run the analysis notebooks:**
```bash
jupyter notebook python_scripts/predictive_model.ipynb
```

**Recreate the SQL views:**
Open any MySQL client, connect to your database, and run the scripts in `sql_scripts/` in order.

---

## Tech Stack

`Python` · `Pandas` · `Matplotlib` · `Seaborn` · `Scikit-Learn` · `MySQL` · `Jupyter`

---

## Data Source

Dataset covers 3 months of transactional sales data across 3 supermarket branches,
including customer type, product line, branch, payment method, and daily sales figures.

---

## License

MIT License — see `LICENSE.md` for details.

---

*Built by [Sihle Kalolo](https://github.com/Toni8) · [Portfolio](https://sihle-kalolo-portfolio.vercel.app/)*
