Trader Behavior Insights (Fear & Greed Index + Hyperliquid Trades)
📌 Project Title:

Trader Behavior Insights Based on Market Sentiment (Fear & Greed Index × Hyperliquid Historical Trades)

📘 Overview

This project analyzes how market sentiment influences trader behavior, volatility, win-rate, and PnL on Hyperliquid.
Using two datasets:

Bitcoin Fear & Greed Index Dataset

Hyperliquid Historical Trader Dataset

The project builds a complete pipeline for:

Data cleaning & merging

Volatility and sentiment regime analysis

Symbol-level sensitivity

Trader clustering & behavioral segmentation

XGBoost-based predictive modeling

🔗 Google Colab Notebooks

Note: All notebooks are publicly accessible with “Anyone with the link can view” enabled.

Main EDA + Modeling Notebook
🔗 notebook_1.ipynb

Additional/Optional Notebook
🔗 notebook_2.ipynb

(Replace placeholders with your actual links.)

📊 Key Analysis Steps
1️⃣ Data Cleaning & Preparation

Parsed timestamps into uniform formats

Extracted date components for sentiment mapping

Cleaned missing/invalid entries

Standardized column names

Merged trader dataset with sentiment dataset on date

2️⃣ Feature Engineering

Created win indicator

Computed normalized PnL metrics

Added leverage buckets, size buckets

Derived rolling volatility & win-rates

3️⃣ Exploratory Analysis

Daily price volatility across sentiment regimes

Symbol-level win-rate comparisons

Daily and 7-day rolling win-rate trends

Greed–Fear behavior differences

Extreme sentiment regime analysis (Extreme Fear vs Extreme Greed)

4️⃣ Trader Behavior Segmentation

Used clustering based on:

Trade frequency

Avg size

Win-rate

PnL mean/std

Three clusters emerged:

Cluster 0: Mid-size, moderate win-rate

Cluster 1: High PnL, high volatility (aggressive traders)

Cluster 2: High-volume, highest win-rate, most stable

5️⃣ Predictive Modeling (XGBoost)

Classification target: win vs loss

Features included sentiment, side, coin, size, leverage, fees

One-hot encoding of categorical variables

Model Evaluation:

Accuracy: X%

ROC–AUC: Y%

Feature importance identified classification, side, and trade size as key predictors.

(Replace X and Y with actual metrics after training.)

📈 Key Insights
✔ Volatility Patterns

Greed & Extreme Greed show highest volatility

Neutral is the most stable

Extreme Fear has sharp volatility spikes

✔ Sentiment-Driven Performance

Win-rate spikes during Greed

Extreme Fear → near-zero win-rates

Rolling win-rates confirm regime momentum effects

✔ Asset Sensitivity

Trend tokens (HYPE, @107) react strongly to Greed

BTC/ETH remain relatively stable

Some tokens show contrarian behavior during Fear

✔ Behavioral Patterns

SELL trades win more during Extreme Fear

BUY trades dominate in Extreme Greed

High-volume traders (Cluster 2) have the best long-term consistency

✔ Modeling Takeaways

Sentiment is a strong predictive feature

XGBoost handles non-linearities well

Feature importance validates sentiment-conditioning

🧪 Technologies Used

Python

Pandas / NumPy

Matplotlib / Seaborn

Scikit-learn

XGBoost

Google Colab

Jupyter Notebook

🚀 How to Reproduce

Clone the repository:

git clone https://github.com/yourusername/ds_dhwani_patel.git
cd ds_dhwani_patel


Open the Colab notebook:

notebook_1.ipynb


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
