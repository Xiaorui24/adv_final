# Advanced DS Final Project
RECS 2020: Energy Cost Analysis and Prediction

This project explores household-level energy cost patterns in the United States using data from the **2020 Residential Energy Consumption Survey (RECS)**. We combine machine learning and nonparametric causal inference techniques to both **predict energy costs** and **evaluate the effect of solar panel adoption**.

## Project Structure

- `analysis/final_project.qmd`: Full Quarto document containing all data cleaning, modeling, and evaluation.
- `data/RECS/recs2020_public_v7.csv`: Raw RECS dataset.

## Data

- **Source**: U.S. Energy Information Administration – RECS 2020 Public Use Microdata
- **Unit**: Household-level
- **Target variable**: `cost` – annual total energy expenditure
- **Key features**: dwelling characteristics, climate zone, appliance usage, income, and solar panel ownership

##  Objectives
1. **Design and evaluate a targeted energy credit policy via microsimulation:**
   - Allocate credits based on household income, energy burden, elderly presence, and medical device usage
   - Estimate policy cost and distributional equity impacts
   - Visualize credit distribution and post-policy cost by income and burden decile

2. **Predict annual household energy cost** using:
   - Lasso Regression
   - Random Forest
   - XGBoost

3. **Assess causal impact of solar panel adoption** on energy costs using:
   - Permutation testing (pre- and post-matching)
   - Nearest-neighbor matching based on income, square footage, year built, and climate zone
