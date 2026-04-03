### NBA Player Position Predictor
# NBA Player Position Predictor

A machine learning project that predicts NBA player positions (Guard, Forward, Center) 
from rate stats alone, using data from the 2024-25 NBA season.

## Overview
Traditional NBA position labels are increasingly misleading in the modern era. This project 
explores whether a player's statistical profile can predict their position — and more 
interestingly, identifies players whose stats don't match their official designation.

## Key Findings
- Both logistic regression and random forest achieved **74% accuracy** on the test set
- Forwards were the hardest position to predict:
every misclassification involved a Forward, never a Center-Guard confusion
- Rebounding was the most important feature by a significant margin
- The model correctly "misclassified" players like Luka Dončić (F->G), Victor Wembanyama (F->C), and Bam Adebayo (C->F) — suggesting it captures how players actually play better than their official NBA labels

## Tech Stack
- Python 3.13
- pandas, numpy
- scikit-learn (Logistic Regression, Random Forest)
- matplotlib, seaborn
- nba_api

## How to Run
1. Clone the repo
2. Install dependencies:
pip install pandas numpy scikit-learn matplotlib seaborn nba_api
3. Open `nba_position_predictor.ipynb` in VS Code or Jupyter
4. Run all cells from top to bottom

## Next Steps
- Test on 2023-24 season data
- Explore 5-class classification (PG, SG, SF, PF, C)
- Extend to multiple seasons for a larger dataset

## Author
Ethan Bracero-Komrosky | UCLA Statistics & Data Science