# 📈 Demand Forecasting for Retail using Prophet

## Overview

Demand forecasting is a critical task in retail analytics that helps businesses optimize inventory management, reduce stockouts, minimize overstocking, and improve supply chain efficiency.

This project uses historical retail sales data and Facebook Prophet, a powerful time-series forecasting library, to predict future sales trends. Additional features such as promotions, customer transactions, and oil prices were incorporated to improve forecasting accuracy.

---

## Problem Statement

Retail businesses often face challenges in accurately predicting future demand due to changing customer behavior, seasonal trends, and external factors.

The objective of this project is to:

* Forecast future product demand using historical sales data.
* Analyze seasonal and trend patterns.
* Support inventory optimization and business decision-making.
* Evaluate forecasting performance using industry-standard metrics.

---

## Dataset

Dataset: **Store Sales - Time Series Forecasting**

**Note:** The original Kaggle dataset files are not included in this repository due to GitHub file size limitations.

### Dataset Source

https://www.kaggle.com/competitions/store-sales-time-series-forecasting

### Features Used

| Feature      | Description                        |
| ------------ | ---------------------------------- |
| date         | Sales date                         |
| sales        | Total sales (Target Variable)      |
| onpromotion  | Number of products under promotion |
| transactions | Customer transaction count         |
| dcoilwtico   | Daily oil price                    |
| year         | Year                               |
| month        | Month                              |
| day          | Day                                |
| dayofweek    | Day of week                        |
| is_weekend   | Weekend indicator                  |

---

## Project Workflow

### 1. Data Collection

Loaded retail sales data and supporting datasets including:

* Sales Data
* Customer Transactions
* Oil Prices
* Holiday Information
* Store Information

### 2. Data Cleaning

* Converted date columns to datetime format.
* Handled missing oil price values using forward-fill and backward-fill techniques.
* Filled missing transaction values.
* Merged multiple datasets into a unified forecasting dataset.

### 3. Exploratory Data Analysis (EDA)

Performed analysis to identify:

* Sales trends over time
* Seasonal patterns
* Weekly demand fluctuations
* Impact of promotions and external factors

### 4. Feature Engineering

Created additional time-based features:

* Year
* Month
* Day
* Day of Week
* Weekend Indicator

### 5. Forecasting Model

Implemented Facebook Prophet with:

* Yearly Seasonality
* Weekly Seasonality
* Trend Detection

### 6. Model Evaluation

Evaluated model performance using:

* Root Mean Squared Error (RMSE)
* Mean Absolute Percentage Error (MAPE)

---

## Model Performance

### RMSE

```text
94,348.20
```

### MAPE

```text
8.26%
```

### Performance Analysis

A MAPE of **8.26%** indicates that the model's predictions differ from actual sales by only about 8% on average, representing excellent forecasting performance for retail demand prediction.

---

## Results

The model successfully captured:

✅ Long-term sales trends

✅ Weekly seasonality patterns

✅ Demand fluctuations over time

✅ Future sales forecasts for the next 90 days

The forecast closely follows actual sales values and demonstrates strong predictive capability.

---

## Visualizations

### Forecasted Sales

<img src="images/forecast_plot.png" width="900">

### Seasonality Components

<img src="images/seasonality_components.png" width="900">

### Actual vs Predicted Sales

<img src="images/actual_vs_predicted.png" width="900">

---

## Power BI Dashboard

In addition to the forecasting model developed using Facebook Prophet, an interactive Power BI dashboard was created to provide business-focused insights and visualize forecasting results.

### Dashboard Pages

#### Executive Overview
- Total Sales KPI
- Average Daily Sales KPI
- Maximum Daily Sales KPI
- Forecast Accuracy (MAPE)
- Historical Sales Trend

#### Sales Analysis
- Monthly Sales Distribution
- Sales by Day of Week
- Demand Pattern Analysis

#### Forecast Analysis
- Actual vs Predicted Sales Comparison
- RMSE Evaluation
- MAPE Evaluation
- Forecast Performance Monitoring

### Dashboard File

The Power BI dashboard file is included in this repository:

```text
PowerBi_dashboard/Demand-Forecasting-Retail.pbix
```

---

## Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Scikit-learn
* Facebook Prophet
* Jupyter Notebook

---

## Project Structure

```text
Demand-Forecasting-Retail/
│
├── data/
│   ├── processed_sales_data.csv
│   └── predictions.csv
│
├── images/
│   ├── forecast_plot.png
│   ├── seasonality_components.png
│   └── actual_vs_predicted.png
│
├── models/
│   └── prophet_model.pkl
│
├── PowerBi_dashboard/
│   └── Demand-Forecasting-Retail.pbix
│
├── demand_forecasting.ipynb
├── requirements.txt
├── README.md
└── .gitignore
```

---

## Future Improvements

* Incorporate holiday effects directly into forecasting.
* Build LSTM-based deep learning forecasting models.
* Forecast demand at the product-category level.
* Develop an interactive Streamlit dashboard.
* Deploy the forecasting model as a web application.

---

## Conclusion

This project demonstrates the practical application of time-series forecasting techniques for retail demand prediction.

By leveraging Facebook Prophet and engineered features, the model achieved strong forecasting performance with a MAPE of **8.26%**, making it suitable for inventory planning and retail decision-making.

The project showcases skills in:

* Data Cleaning
* Feature Engineering
* Time-Series Forecasting
* Model Evaluation
* Data Visualization

and serves as a strong portfolio project for Data Science, Data Analytics, and Machine Learning roles.

---

## Author

**Ajinkya Mariche**

Data Science Intern Project

GitHub: https://github.com/Ajinkya7890
