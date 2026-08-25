# Investment KPI & ROI Tracking System

An Excel-based financial analytics system that tracks, analyzes, and visualizes the performance of a corporate investment portfolio — built as a non-coding (formula-only) FP&A / Investment Analytics project, with a companion interactive web dashboard.

**[🔴 Live Dashboard]**



https://github.com/user-attachments/assets/a084cdfe-941f-44cc-8a2d-db4676e7e0c1




· **[Download the full workbook Below](financial-model/Investment_KPI_ROI_Tracking_System.xlsx)** · 150 investments · 9 linked worksheets · fully formula-driven

https://1drv.ms/x/c/d25b756fc27d4ee3/IQDfT4GYso0eTYGqulQGVnrYAReORgSoo6-gzyZhN_660Qk?e=w686jN


## What this is

A simulated corporate investment portfolio (150 investments across 10 categories, 8 departments and 5 regions) tracked from initial budget through to actual return, with automatic calculation of ROI, NPV, IRR, Payback Period, Budget Variance, Risk classification, and a Best/Base/Worst case scenario model — all built with native Excel formulas (no macros, no VBA, no code).

## Why

Capital allocation decisions shouldn't rely on a single number. This project shows how to combine **return** (ROI, NPV, IRR), **risk** (a Risk-Return quadrant), and **budget discipline** (Budget vs Actual variance) into one decision-support tool, the way an FP&A or investment analytics team would.

## Repository structure

```
investment-kpi-roi-tracking/
├── financial-model/
│   └── Investment_KPI_ROI_Tracking_System.xlsx   # the full workbook (9 sheets)
├── data/
│   └── investment_data.csv                       # raw dataset export (150 records)
├── dashboard/
│   └── index.html                                 # standalone interactive web dashboard
├── screenshots/
│   └── (dashboard & sheet screenshots go here)
├── docs/
│   └── methodology.md                             # KPI formulas & assumptions explained
└── README.md
```

## Running the interactive dashboard

The `dashboard/index.html` file is a **self-contained, no-build, no-dependency** web dashboard — the KPI data is embedded directly in the file, so it works two ways:

**Locally:** just download `dashboard/index.html` and open it in any browser.

**Live on the web (recommended for sharing):**
1. Push this repo to GitHub
2. Go to **Settings → Pages** → set source to your `main` branch
3. GitHub will publish it at `https://YOUR-USERNAME.github.io/investment-kpi-roi-tracking/dashboard/`
4. Update the live link at the top of this README with your real URL

The dashboard has 5 tabs (Categories, Departments, Budget vs Actual, Risk & Return, Scenario Analysis), sortable tables, and a live KPI ticker — all built in plain HTML/CSS/JS.

## Workbook contents

| Sheet | What it shows |
|---|---|
| **Dashboard** | KPI cards + 6 charts: ROI by category, Target vs Actual ROI, Department investment, Budget vs Actual, Risk-Return quadrants, Performance Rating distribution |
| **Raw_Data** | 150 investment records with full input + formula columns (ROI, NPV, IRR, Payback, Performance Rating, Decision Recommendation) |
| **KPI_Summary** | 19 portfolio-level KPIs |
| **ROI_Analysis** | ROI, NPV and ranking by investment category |
| **NPV_IRR** | NPV and IRR rollups by category |
| **Budget_vs_Actual** | Cost overrun tracking by category |
| **Department_Analysis** | Capital allocation and returns by department |
| **Risk_Return** | Four-quadrant risk/return classification |
| **Scenario_Analysis** | Editable Best/Base/Worst case assumptions with live portfolio ROI recalculation |


## Key insights from this dataset

- **Portfolio scale:** $812.5M total actual investment against $715.7M budgeted — a **13.5% cost overrun** overall
- **Average ROI:** 13.7% actual vs. 19.6% average target — the portfolio is **underperforming target by ~6 points** on average
- **Best-performing category:** Technology (36.8% avg ROI), followed by Digital Transformation (24.1%)
- **Weakest categories:** Acquisition Projects (-10.8% avg ROI) and Automation (-4.9%) — both net negative
- **Best-performing department:** Product (25.5% avg ROI on $133.8M invested), followed by Sales (23.2%)
- **Weakest department:** HR (2.5% avg ROI on $131.1M invested) — high spend, low return
- **Risk-Return split:** 46 investments sit in High Return / Low-Medium Risk (the ideal quadrant); 27 sit in Low Return / High Risk (the ones to review first)
- **Rating distribution:** 56 investments rated "Excellent," 83 rated "Critical" — meaning a majority of the portfolio needs review or restructuring

*(These are generated from a synthetic dataset seeded for reproducibility — see [`docs/methodology.md`](docs/methodology.md) for how it was built.)*

## Tools used

Microsoft Excel — formulas only (SUMIF/SUMIFS, AVERAGEIF/AVERAGEIFS, SUMPRODUCT, INDEX/MATCH, NPV logic, conditional formatting, data validation, native charts). No add-ins, no VBA.

## Author

Heena Siddiqui
heenasiddiqui782@gmail.com
www.linkedin.com/in/heenasiddiqui



