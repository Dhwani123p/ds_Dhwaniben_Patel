**Trader Behavior Insights (Fear & Greed Index + Hyperliquid Trades)
**

📌 Project Title:

Trader Behavior Insights Based on Market Sentiment (Fear & Greed Index × Hyperliquid Historical Trades)

📘 Overview

This project analyzes how market sentiment influences trader behavior, volatility, win-rate, and PnL on Hyperliquid.
Using two datasets:

1. Bitcoin Fear & Greed Index Dataset

2. Hyperliquid Historical Trader Dataset

The project builds a complete pipeline for:

a.Data cleaning & merging

b.Volatility and sentiment regime analysis

c.Symbol-level sensitivity

d.Trader clustering & behavioral segmentation

e.XGBoost-based predictive modeling

🔗 Google Colab Notebooks

Note: All notebooks are publicly accessible with “Anyone with the link can view” enabled.

Main EDA + Modeling Notebook
🔗[ notebook_1.ipynb](https://colab.research.google.com/drive/1gwXHTVx9GhK_jA-Vi5RYtq6bQ8FXr6ps?usp=sharing)


(Replace placeholders with your actual links.)

📊 Key Analysis Steps
1️⃣ Data Cleaning & Preparation

a. Parsed timestamps into uniform formats

b. Extracted date components for sentiment mapping

c. Cleaned missing/invalid entries

d. Standardized column names

e. Merged trader dataset with sentiment dataset on date

2️⃣ Feature Engineering

a. Created win indicator

b. Computed normalized PnL metrics

c. Added leverage buckets, size buckets

d. Derived rolling volatility & win-rates

3️⃣ Exploratory Analysis

a. Daily price volatility across sentiment regimes

b. Symbol-level win-rate comparisons

c. Daily and 7-day rolling win-rate trends

d. Greed–Fear behavior differences

e. Extreme sentiment regime analysis (Extreme Fear vs Extreme Greed)

4️⃣ Trader Behavior Segmentation

a. Used clustering based on:

b. Trade frequency

c. Avg size

d. Win-rate

e. PnL mean/std

f. Three clusters emerged:

  i. Cluster 0: Mid-size, moderate win-rate

  ii. Cluster 1: High PnL, high volatility (aggressive traders)

  iii. Cluster 2: High-volume, highest win-rate, most stable




🧪 Technologies Used

Python

Pandas / NumPy

Matplotlib / Seaborn

Scikit-learn

Google Colab

Jupyter Notebook

🚀 How to Reproduce

Clone the repository:

git clone https://github.com/dhwani123p/ds_dhwaniben_patel.git

cd ds_dhwaniben_patel


Open the Colab notebook:

[notebook_1.ipynb
](https://colab.research.google.com/drive/1gwXHTVx9GhK_jA-Vi5RYtq6bQ8FXr6ps?usp=sharing)

Ensure uploaded datasets match structure used in code

Run all cells top–to–bottom

All generated charts will automatically appear in:

outputs/


🏁 About the Author


Dhwaniben Patel

Aspiring Machine Learning & Data Science Engineer

Focused on quantitative analysis, NLP, and real-time trading intelligence.

Trend discovery & actionable insights

All findings are supported by visualizations saved in the /outputs directory and intermediate data in /csv_files.
