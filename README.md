# Factors Contributing to House Prices in the United States (2020–2024)

## Team Members
Brody Hughson, Cesar Fontanelli, Marris Jones, Pedro Liriano

## Project Goal
Analyze which factors are most associated with U.S. home prices (2020–2024) using merged public datasets and predictive modeling.

## Data Sources
- U.S. Census Population Estimates (cities/towns)
- Zillow Home Value Index (ZHVI)
- Zillow Observed Rent Index (ZORI)
- Residential Construction Permits by County
- ACS 5-Year Housing Estimates by State
- FRED: 30-Year Fixed Rate Mortgage Average in the United States (MORTGAGE30US)

## Repository Structure
- `IDS Group 2 Project Report.ipynb` — main analysis notebook
- `Data/` — raw and cleaned project datasets
- `requirements.txt` — Python dependencies
- `DATA_DICTIONARY.md` — column definitions and units

## Setup
```bash
python -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
```

## Run
```bash
jupyter notebook
```
Open `IDS Group 2 Project Report.ipynb` and run all cells from top to bottom.

## Methods Summary
1. Data ingestion and cleanup for each dataset.
2. Feature engineering (per-capita rates, encoding, and scaling).
3. Dataset merge on geography + time.
4. Exploratory data analysis (EDA).
5. Modeling (baseline linear regression, decision tree, random forest, gradient boosting).
6. Feature importance and model interpretability.
7. Model comparison + conclusions.

## Deliverables
- Completed notebook with EDA + modeling
- Cleaned datasets and metadata
- Report + slide draft (see `reports/` and `slides/`)
