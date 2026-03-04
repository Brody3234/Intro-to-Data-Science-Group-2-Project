# Factors Contributing to House Prices in the United States

## Team Members
Brody Hughson, Cesar Fontanelli, Marris Jones, Pedro Liriano

## Project Goal
Analyse which factors are most associated with U.S. home prices (2020-2024) using merged public datasets and predictive modeling.

## Data Sources
-U.S. Census Population Estimates (citis/towns)
-Zillow Home Value Index (ZHVI)
-Zillow Observed Rent Index (ZORI)
-Residential Construction Premits by County
-ACS 5-Year Housing Estimates by State
-Fred 30-Year Housing Estimates by Sate

## Repository Files
- 'IDS Group 2 Project Report.ipynb' - main analysis notebook
- 'Data/' = project datasets

## Setup
'''bash
python -m venv .venv
source .venv/bin/activate
pip install -r requirments.txt
'''

## Run
'''bash
jupyter notebook
'''

Then open 'IDS Group 2 Project Report.ipynb' and run all cells from top to bottom.

## Methods Summary
-data cleaning and null handling
-Year-level feature engineering (2020-20204)
-Inter-table merges by city/state/year
-Exploratory data analysis and trend charts
-Model comparison: Linear Regression, Random Forcest, Gradient Boosting

## Deliverables
-Final notebook with outputs
-exported PDF/HTML report
-Slide deck with key findings

## Personal Contributions (fill in before subissions)
-Added final findings and conclusion text
-Added model comparison summary table
Documented data limitations and assumptions 
Created README with setup/run instructions
