# Historical_Trader_Data
# Trader Behavior and PnL Analysis using Machine Learning and Explainable AI

## How to Run the Project (Jupyter Notebook)

- Clone the repository to your local system  
- Open the Jupyter Notebook file (`.ipynb`)  
- Ensure Python version 3.9 or above is installed  
- Install the required dependencies:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn xgboost shap
```

---

## End-to-End Approach
# 1. Data Understanding and Preparation

Performed checks for:

Missing values

Duplicate records

Timestamp inconsistencies

Converted timestamps and extracted:

Hour of trade

Day of week

This enabled time-based behavioral analysis

# 2. Feature Engineering

Key engineered features:

Trade size in USD

Absolute PnL (risk magnitude)

Fee ratio as an indicator of over-trading

Win rate

Trade frequency

These features helped capture how traders make decisions and take risk

# 3. Exploratory Data Analysis

I performed detailed exploratory analysis using visualizations to study:

PnL distribution

Buy versus sell performance

Long versus short risk profiles

Relationship between trade size and PnL

Initial analysis showed that higher trade sizes increase volatility and over-trading does not ensure profitability

# 4. Model Selection
Why XGBoost

Trading data is tabular, noisy, and highly non-linear

XGBoost is well suited for:

Tabular datasets

Capturing complex feature interactions

Robust and efficient model performance

I used XGBoost for:

PnL prediction

PnL volatility prediction

Why LSTM

LSTM was used for comparison with traditional machine learning

It is effective for capturing sequential and temporal patterns

Results showed:

LSTM captures smooth trends

XGBoost performs better for sharp changes in PnL

This comparison strengthened the final model choice

# 5. Volatility Modeling

Volatility represents:

Risk exposure

Stability of trading behavior

Trader discipline

This makes the analysis more relevant for real-world risk management

# 6. Trader Clustering and Behavioral Archetypes

Clustering was based on:

Average PnL

Volatility

Win rate

Trade frequency

This segmentation helped identify distinct behavioral archetypes such as:

Consistent performers

Over-traders

High-risk opportunistic traders

# 7. Explainable AI using SHAP

SHAP analysis showed that:

Trade size and fee intensity are the strongest drivers of volatility

Time-based features have relatively lower influence

# 8. Actionable Outcomes

Implement behavioral alerts for over-trading

Incentivize low-volatility and consistent traders

Use trader clustering for personalized risk and leverage controls
