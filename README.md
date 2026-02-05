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

<img width="1108" height="503" alt="image" src="https://github.com/user-attachments/assets/715960f5-ad04-459d-a5af-75ccbe6ac39e" />
<img width="1100" height="496" alt="image" src="https://github.com/user-attachments/assets/af9a8a4e-a97a-4ccb-b083-917eaf52d65f" />
<img width="911" height="583" alt="image" src="https://github.com/user-attachments/assets/2150ee12-bb39-43f5-935e-f3891cfab0b2" />
<img width="718" height="496" alt="image" src="https://github.com/user-attachments/assets/27616aaf-1c8a-456f-9bcd-89e44b422848" />
<img width="798" height="486" alt="image" src="https://github.com/user-attachments/assets/4e080873-a191-4efb-b988-70e7d906891b" />
<img width="900" height="672" alt="image" src="https://github.com/user-attachments/assets/6906ef3a-2726-4d1c-89ee-0217d557dcfd" />
<img width="1108" height="509" alt="image" src="https://github.com/user-attachments/assets/13005b41-07c6-4766-972a-9a8dedc98096" />
<img width="1107" height="419" alt="image" src="https://github.com/user-attachments/assets/5724b760-60ee-4aef-aaca-f15adf19fb26" />
<img width="689" height="480" alt="image" src="https://github.com/user-attachments/assets/2ac8e56b-b2a3-4bf4-abbd-ab24d8487005" />
<img width="1031" height="578" alt="image" src="https://github.com/user-attachments/assets/706d16e9-9cb9-43e8-812c-fbe5af1ec439" />
<img width="1105" height="602" alt="image" src="https://github.com/user-attachments/assets/1db88cca-8fee-45d5-ad6e-cc592a7880f5" />
<img width="1084" height="449" alt="image" src="https://github.com/user-attachments/assets/9d7c630e-27ec-4a34-b09c-a651043a8d0a" />
<img width="957" height="667" alt="image" src="https://github.com/user-attachments/assets/2d9a880a-3849-431d-84e4-8dcf21b5d44b" />

