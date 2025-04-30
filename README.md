
# 🛒 Costco Sales Forecasting Using Machine Learning

![Costco Forecasting Banner](https://raw.githubusercontent.com/VishalAnton20/Costco-Sales-Analysis/main/img.jpg) <!-- Replace with your actual image link -->

## 📌 Project Overview

This project focuses on building machine learning models to predict weekly sales for Costco stores across the US. By leveraging historical sales data, economic indicators, and holiday effects, the models aim to forecast demand more accurately, helping Costco optimize inventory planning, promotional strategies, and staffing.

## 🧠 Business Context

Costco operates numerous stores across diverse regions, each influenced by local economic conditions and seasonal trends. Unpredictable demand surges, especially during holidays and promotions, have previously led to stockouts or overstocking. The primary goal is to develop robust ML models that can capture these complex relationships and improve forecast reliability.

## 🗂️ Dataset Description

| Feature          | Description                                                        |
|------------------|--------------------------------------------------------------------|
| `Store`          | Unique ID for each store                                           |
| `Date`           | Week-ending date for sales                                         |
| `Weekly_Sales`   | Weekly revenue for a given store                                   |
| `Holiday_Flag`   | Binary flag (1 = holiday week, 0 = non-holiday)                    |
| `Temperature`    | Average temperature during the week                                |
| `Fuel_Price`     | Average regional fuel price                                        |
| `CPI`            | Consumer Price Index                                               |
| `Unemployment`   | Unemployment rate in the store's region                            |

🗓 **Holiday Events Included:**
- Super Bowl
- Labour Day
- Thanksgiving
- Christmas

## 🎯 Objectives

- Perform Exploratory Data Analysis (EDA) to uncover trends and seasonality.
- Engineer time-based and economic features to boost model performance.
- Apply and compare regression models:  
  Linear Regression, Ridge, Lasso, Random Forest, XGBoost.
- Evaluate using RMSE, R², MAE.
- Interpret results using SHAP (SHapley Additive Explanations).
- Generate actionable business insights for decision-making.

## 📊 Exploratory Data Analysis

- Trends in sales over time
- Holiday vs. non-holiday week comparisons
- Correlation matrix of features
- Seasonal and store-wise analysis

## ⚙️ Models & Techniques Used

| Model               | Techniques Applied                              |
|---------------------|--------------------------------------------------|
| Linear Regression   | Baseline model                                  |
| Ridge & Lasso       | Regularization to prevent overfitting           |
| Random Forest       | Ensemble model capturing non-linear patterns    |
| XGBoost             | Gradient boosting for high performance          |

Evaluation metrics:
- RMSE (Root Mean Squared Error)
- MAE (Mean Absolute Error)
- R² Score

📌 SHAP analysis highlighted:
- Store ID and Month as major contributors.
- CPI and Fuel Price had limited predictive power in this dataset.

## 💡 Business Insights

- Holiday weeks significantly spike sales; including event context improves forecasts.
- Regional promotions could be optimized using store-level seasonal trends.
- Recommend enriching the dataset with demographic and regional metadata for improved accuracy.

## 🛠️ Tech Stack

- **Python** (Pandas, NumPy, Scikit-learn, XGBoost, SHAP, Matplotlib, Seaborn)
- **Jupyter Notebook / Google Colab**
- **Git & GitHub**

## 📂 Project Structure

```
📁 Costco-Sales-Forecasting/
├── Costco_Sales_Enhanced_Deep_Analysis.ipynb
├── README.md
├── images/
│   └── Costco-banner.jpg
├── Costco_Store_sales.csv
└── requirements.txt
```

## 🚀 Future Work

- Implement time-series forecasting using Facebook Prophet or ARIMA.
- Deploy the model using Flask or Streamlit.
- Integrate dashboard with Power BI or Tableau for business users.
- Automate retraining pipeline with Airflow.
