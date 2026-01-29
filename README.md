# 📊 Forecasting Video Games Inventory Sales

<img width="1519" height="2000" alt="image" src="https://github.com/user-attachments/assets/c149dd39-bc5f-4521-a328-8dee16e48005" />


Forecast monthly video game sales to help optimize inventory management for a reseller or retailer.

Accurate forecasting ensures adequate stock levels, reduces costs of overstock, and ensures products are available when customers want them.

---

## 📌 Project Overview

This project contains a complete analysis and forecasting workflow for video game inventory sales:
- Data loading and cleaning
- Exploratory Data Analysis (EDA)
- Feature engineering
- Model training & evaluation
- Insights & interpretation

This helps businesses make data-driven decisions to balance inventory with expected demand.

---

## 📁 Dataset

The dataset includes monthly sales data for video games:
- `monthly_sales_data.csv` — raw sales data
- `clean_monthly_sales_data.csv` — cleaned and formatted for forecasting

Each record includes:
- Date/month of sale
- Total units sold  
  Category,	Month,	Sales	Year,	DayOfWeek,	Platform,	Holiday,	Promotion,	Quarte*

---

## 🧠 Tools & Technologies

| Component | Tools |
|-----------|-------|
| Language  | Python |
| Notebook  | Jupyter / Google Colab |
| Libraries | Pandas, NumPy, Matplotlib, Seaborn, Scikit-Learn |
| Forecasting Models | ( ARIMA , ETS |

---

## 🔎 Methodology

1. **Data Preparation**
   - Load data
   - Convert dates to datetime format
   - Handle missing values

2. **Exploratory Data Analysis**
   - Plot sales trends over time
   - Identify seasonal patterns
   - Examine sales volatility

3. **Feature Engineering**
   - Create lag features
   - Rolling averages
   - Time components (month, year)

4. **Model Training**
   - Train forecasting models (e.g., ARIMA / ETS)
   - Tune hyperparameters

5. **Evaluation**
   - Compare model performance using MAE / RMSE
   - Validate on test set

---

## 📈 Results and Insights

| Model   | Train RMSE | Test RMSE |
|---------|------------|-----------|
| 0  ARIMA  |30307.257416 |25187.767836 |
| 1    ETS  |31772.046436 |24549.700275 |


### 📈 Model Results & 4-Month Forecast

**Model Selection:**  
Based on the evaluation of forecasting models, **ARIMA** was chosen because it achieved a slightly lower **Root Mean Squared Error (RMSE)** compared to the ETS model, indicating a better fit to the test data.

**4-Month Sales Forecast:**

| Month       | Forecasted Sales |
|------------|-----------------|
| 2024-01-01 | 114,233         |
| 2024-02-01 | 112,433         |
| 2024-03-01 | 111,662         |
| 2024-04-01 | 111,332         |

**Business Implications:**  
- **Inventory Management:** Adjust orders to prevent overstocking while aligning with the forecasted stable trend.  
- **Resource Optimization:** Reallocate staffing, production, and logistics according to projected sales.  
- **Sales & Marketing:** Refine strategies to address forecasted demand and explore opportunities to stimulate sales.  
- **Financial Planning:** Integrate the forecast into revenue projections and budgeting for improved accuracy.

> **Insight:** The forecast indicates a slight, steady decline in sales over the next four months. Leveraging this forecast allows informed decision-making, proactive planning, and continuous adaptation to market trends to maximize profitability.

