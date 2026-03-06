# Factors Contributing to House Prices in the United States

## Team Members
Brody Hughson, Cesar Fontanelli, Marris Jones, Pedro Liriano, Jeremiah Tatum

## Project Goal
Analyze which factors are most associated with U.S. home prices (2020-2024) using merged public datasets and predictive modeling.

## Data Sources
- U.S. Census Population Estimates (cities/towns)
- Zillow Home Value Index (ZHVI)
- Zillow Observed Rent Index (ZORI)
- Residential Construction Permits by County
- ACS 5-Year Housing Estimates by State
- FRED 30-Year Housing Estimates by State

## Repository Files
- \ IDS Group 2 Project Report.ipynb' - main analysis notebook
- \ Data/' - project datasets'

## Setup
'''bash
python -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
'''

## Run
'''bash
jupyter notebook
'''

Then open \'IDS Group 2 Project Report.ipynb\' and run all cells from top to bottom.

## Methods Summary
- Data cleaning and null handling
- Year-level feature engineering (2020-2024)
- Inter-table merges by city/state/year
- Exploratory data analysis and trend charts
- Model comparison: Linear Regression, Random Forest, Gradient Boosting

## Deliverables
- Final notebook with outputs
- Exported PDF/HTML report
- Slide deck with key findings
