# IPL Match Intelligence Dashboard

An end-to-end data analytics and machine learning project built on IPL match data from 2008 to 2024, covering exploratory data analysis, statistical insights, predictive modeling, and an interactive Power BI dashboard.

## Tech Stack
Python, Pandas, NumPy, Matplotlib, Seaborn, scikit-learn, Power BI

## Dataset
IPL Complete Dataset (2008-2024) by patrickb1912 on Kaggle
Source: Cricsheet

## Project Structure
- `ipl_analysis.ipynb` — Main notebook with EDA and ML model
- `IPL_Dashboard.pbix` — Power BI dashboard file
- `*.png` — Exported chart visualizations

## Analysis Performed
- Top 10 run scorers across all IPL seasons
- Most wins by team (2008-2024)
- Toss impact on match result
- Top venues by matches hosted
- Most Player of the Match awards

## Machine Learning Model
Built a Random Forest Classifier to predict match winners based on team composition, toss outcome, toss decision, and venue.

- Algorithm: Random Forest (100 estimators)
- Features: team1, team2, toss_winner, toss_decision, venue
- Accuracy: 48% on test set
- Baseline (random guess): ~6-7% across 15+ team classes

The model significantly outperforms random baseline. Lower accuracy reflects the inherent unpredictability of cricket outcomes rather than a modeling flaw.

## Power BI Dashboard
The dashboard visualizes key IPL statistics across four panels: team win counts, player of the match leaders, toss impact analysis, and venue-wise match distribution.

## How to Run
1. Download matches.csv and deliveries.csv from the Kaggle dataset linked above
2. Place them in the same directory as the notebook
3. Run all cells in `ipl_analysis.ipynb`
