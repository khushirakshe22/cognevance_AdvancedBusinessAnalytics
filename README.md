# Advanced Business Data Analytics System

## Cognevance Technologies — Data Analysis with Python

An end-to-end business analytics project developed using Python to analyze large-scale retail transaction data, identify business trends, analyze customer behavior, generate KPIs, perform predictive analytics, and produce actionable business insights.

---

## 📌 Project Overview

This project focuses on building an Advanced Business Data Analytics System using a large-scale retail transaction dataset.

The project covers the complete analytics workflow:

- Data collection and ingestion
- Data preprocessing and cleaning
- Feature engineering
- Exploratory Data Analysis (EDA)
- KPI analysis
- Revenue trend analysis
- Customer behavior analysis
- Country-wise business analysis
- Predictive analytics
- Model evaluation
- Predictive insights
- Business recommendations
- Data visualization
- Analytics workflow documentation

---

## 🎯 Project Objectives

The main objectives of this project are:

1. Collect and analyze a large-scale business dataset.
2. Perform advanced data preprocessing and data validation.
3. Handle missing values, duplicate records, and invalid values.
4. Perform feature engineering for business analysis.
5. Analyze business trends and key performance indicators.
6. Understand customer purchasing behavior.
7. Develop a predictive revenue forecasting model.
8. Evaluate the predictive model using appropriate metrics.
9. Generate predictive insights and business recommendations.
10. Document the complete analytics workflow and architecture.

---

## 📊 Dataset

### Online Retail II Dataset

**Source:** UCI Machine Learning Repository

The dataset contains retail transaction records covering approximately two years.

### Original Dataset

- Records: 1,067,371
- Columns: 8

### Original Columns

- Invoice
- StockCode
- Description
- Quantity
- InvoiceDate
- Price
- Customer ID
- Country

### Final Analytical Dataset

After data cleaning and preprocessing:

- Records: 779,425
- Columns: 18
- Missing values: 0
- Duplicate records: 0

---

## 🧹 Data Preprocessing

The following preprocessing operations were performed:

### Duplicate Removal

- Duplicate records removed: 34,335

### Missing Value Handling

Missing values were identified in:

- Description
- Customer ID

Records with missing Description or Customer ID were removed for reliable customer and product analysis.

### Invalid Data Handling

The following invalid records were removed:

- Quantity ≤ 0: 18,390
- Price ≤ 0: 70

### Final Data Quality

- Missing values: 0
- Duplicate records: 0
- Invalid Quantity values: 0
- Invalid Price values: 0

---

## ⚙️ Feature Engineering

A new revenue feature was calculated:

`Revenue = Quantity × Price`

Additional time-based features were created:

- Year
- Month
- Month_Name
- Quarter
- Day
- DayOfWeek
- Day_Name
- Hour
- Is_Weekend

These features were used for trend analysis, KPI analysis, customer analysis, and predictive analytics.

---

## 🛠️ Technologies and Libraries

### Programming Language

- Python

### Libraries

- Pandas
- NumPy
- Matplotlib
- Scikit-learn

### Development Environment

- Google Colab
- GitHub

---

## 📈 KPI Analysis

The major business KPIs identified from the cleaned dataset are:

| KPI | Value |
|---|---:|
| Total Revenue | 17,374,804.27 |
| Total Quantity Sold | 10,513,952 |
| Total Transactions | 36,969 |
| Total Customers | 5,878 |

---

## 📊 Business Trend Analysis

### Year-wise Revenue

| Year | Revenue |
|---|---:|
| 2009 | 683,504.01 |
| 2010 | 8,374,496.09 |
| 2011 | 8,316,804.16 |

### Monthly Revenue Analysis

- Highest revenue month: November
- Highest monthly revenue: 2,322,665.63
- Lowest revenue month: February
- Lowest monthly revenue: 950,643.88

The analysis shows strong revenue activity during the later months of the year, particularly around October and November.

---

## 👥 Customer Behavior Analysis

Customer purchasing behavior was analyzed using:

- Transaction frequency
- Customer revenue contribution
- Top customer identification

### Key Findings

- Most frequent customer: Customer ID 14911
- Number of transactions: 398
- Highest revenue customer: Customer ID 18102
- Customer revenue: 580,987.04

This analysis helps identify high-value and frequently purchasing customers.

---

## 🌍 Country-wise Business Analysis

Revenue was also analyzed across different countries.

### Top Revenue Country

**United Kingdom**

Revenue generated:

**14,389,234.92**

Other major contributing countries include:

- EIRE
- Netherlands
- Germany
- France
- Australia
- Spain
- Switzerland
- Sweden
- Denmark

---

## 🤖 Predictive Analytics

A revenue forecasting model was developed using **Scikit-learn Linear Regression**.

The forecasting model used:

- Year
- Month

as input features to predict monthly revenue.

### Dataset Split

- Training period: 20 months
- Testing period: 5 months

### Model Evaluation

| Metric | Result |
|---|---:|
| R² Score | -0.1830 |
| RMSE | 262,374.67 |
| Average Prediction Error | 29.84% |

The model provides a baseline forecasting approach. The evaluation results indicate that more advanced time-series forecasting techniques could improve prediction accuracy.

---

## 🔮 Predictive Insights

The model was evaluated on the final five months of the dataset.

Key observations:

- November recorded the highest actual revenue during the test period.
- The model underestimated revenue during September, October, and November.
- The model overestimated December revenue.
- The average prediction error was approximately 29.84%.

These results demonstrate the importance of using more advanced forecasting techniques for improved business prediction accuracy.

---

## 💡 Business Recommendations

Based on the analysis:

1. Focus inventory and marketing efforts on high-revenue periods.
2. Prepare inventory in advance of peak sales periods.
3. Monitor and retain high-frequency customers.
4. Prioritize high-value customers through targeted strategies.
5. Track important business KPIs regularly.
6. Use predictive analytics as a planning support tool.
7. Improve future forecasting using advanced time-series models.

---

## 📊 Visualizations

The project includes the following visualizations:

1. Year-wise Revenue
2. Monthly Revenue Trend
3. KPI Summary
4. Top Customers by Revenue
5. Customer Transaction Frequency
6. Country-wise Revenue
7. Actual vs Predicted Revenue

All visualization files are available in the `visualizations/` directory.

---

## 🔄 Analytics Workflow

```text
Business Dataset
       ↓
Data Collection
       ↓
Data Ingestion
       ↓
Data Cleaning & Preprocessing
       ↓
Data Validation
       ↓
Feature Engineering
       ↓
Exploratory Data Analysis
       ↓
KPI & Trend Analysis
       ↓
Customer Behavior Analysis
       ↓
Country-wise Analysis
       ↓
Predictive Analytics
       ↓
Model Evaluation
       ↓
Predictive Insights
       ↓
Business Recommendations
       ↓
Visualizations & Reporting
