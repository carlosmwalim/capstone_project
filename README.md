# 📊 Retail Sales Data Analytics & Revenue Prediction

## 📌 Project Overview

This project demonstrates an end-to-end retail sales analytics workflow using Python. The analysis explores sales performance across different regions and product categories, performs data cleaning and feature engineering, creates insightful visualizations, and develops a machine learning model to predict net revenue.

The project simulates a real-world business intelligence scenario where sales data is transformed into actionable insights that support strategic decision-making.

---

# 🎯 Objectives

The main objectives of this project are to:

- Explore and understand retail sales data.
- Assess and improve data quality.
- Handle missing values.
- Engineer new business features.
- Analyze sales trends across regions and product categories.
- Visualize business performance.
- Build a predictive machine learning model.
- Evaluate model accuracy using multiple metrics.

---

# 📂 Dataset

The dataset contains **1,200 retail sales transactions** recorded between **2022 and 2024**.

### Features

- Date
- Region
- Product Category
- Units Sold
- Unit Price
- Revenue
- Discount Percentage

After feature engineering, additional variables include:

- Year
- Month
- Net Revenue

---

# 🛠 Tools & Technologies

- Python
- Google Colab
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

---

# 📈 Project Workflow

## 1. Data Loading

- Imported required Python libraries.
- Loaded the CSV dataset into a Pandas DataFrame.
- Inspected the first and last records.
- Examined dataset structure and summary statistics.

---

## 2. Data Exploration

Performed:

- Dataset shape inspection
- Data type analysis
- Missing value analysis
- Descriptive statistics

### Findings

- Dataset contains **1,200 records**.
- Missing values exist only in the **Discount Percentage** column.
- Revenue and pricing variables show significant variation across transactions.

---

## 3. Data Cleaning

The following preprocessing steps were performed:

- Filled missing discount values using the median.
- Converted the Date column to datetime format.
- Extracted Year and Month.
- Calculated Net Revenue after discounts.

---

## 4. Feature Engineering

Created new variables including:

### Year

Extracted from transaction date.

### Month

Used for trend analysis.

### Net Revenue

Calculated using:

```
Net Revenue = Revenue × (1 − Discount Percentage)
```

### One-Hot Encoding

Converted categorical variables into numerical features for machine learning.

---

# 📊 Exploratory Data Analysis

Six visualizations were created.

---

## 1. Monthly Net Revenue by Region

Shows how sales changed over time across different regions.

**Business Insight**

- Compare regional performance.
- Identify high-performing regions.
- Monitor seasonal sales trends.

---

## 2. Average Units Sold by Product Category

Compares product demand.

**Business Insight**

- Identify popular product categories.
- Improve inventory planning.

---

## 3. Revenue Distribution by Region

Boxplot showing revenue variation.

**Business Insight**

- Detect regional outliers.
- Understand sales consistency.

---

## 4. Units Sold vs Net Revenue

Regression scatter plot showing the relationship between sales volume and revenue.

**Business Insight**

- Higher sales volumes generally generate higher net revenue.

---

## 5. Correlation Heatmap

Shows relationships between numerical variables.

**Business Insight**

- Identify variables useful for predictive modeling.
- Understand feature relationships.

---

## 6. Total Net Revenue by Product Category

Ranks product categories by revenue.

**Business Insight**

- Identify top-performing product categories.
- Support marketing and inventory decisions.

---

# 🤖 Machine Learning

A **Linear Regression** model was developed to predict **Net Revenue**.

## Feature Selection

Model inputs included:

- Units Sold
- Unit Price
- Discount Percentage
- Year
- Month
- Region (encoded)
- Product Category (encoded)

Target Variable:

- Net Revenue

---

## Model Training

The dataset was divided into:

- 80% Training
- 20% Testing

A Linear Regression model was trained using Scikit-learn.

---

# 📈 Model Evaluation

Performance metrics:

| Metric | Value |
|---------|-------:|
| R² Score | **0.95** |
| MAE | **3430.79** |
| RMSE | **4962.41** |

### Interpretation

- The model explains approximately **95% of the variation** in Net Revenue.
- Low prediction errors indicate strong model performance.
- The model demonstrates that business revenue can be accurately predicted using historical sales features.

---

# 📉 Actual vs Predicted Analysis

A scatter plot comparing actual and predicted values was created.

### Result

Most observations lie close to the diagonal reference line, indicating that the model predicts Net Revenue with high accuracy.

---

# 📊 Key Business Insights

- Revenue varies across different regions.
- Some product categories consistently outperform others.
- Higher sales volumes generally produce higher revenue.
- Discount strategies directly affect Net Revenue.
- Correlation analysis helps identify variables important for forecasting.
- Predictive analytics can support sales planning and budgeting.

---

# 💼 Business Value

This project demonstrates how retail organizations can:

- Monitor regional sales performance.
- Evaluate product category profitability.
- Optimize pricing and discount strategies.
- Improve inventory management.
- Forecast future revenue using machine learning.
- Support data-driven business decisions.

---

# 📁 Repository Structure

```
Retail-Sales-Analytics/
│
├── data/
│   └── Capstone_Project_data.csv
│
├── notebook/
│   └── Capstone_Project.ipynb
│
├── charts/
│   ├── monthly_net_revenue.png
│   ├── units_by_category.png
│   ├── revenue_distribution.png
│   ├── units_vs_revenue.png
│   ├── correlation_heatmap.png
│   ├── revenue_by_category.png
│   └── actual_vs_predicted.png
│
├── images/
│   └── project_preview.png
│
├── README.md
├── requirements.txt
└── LICENSE
```

---

# 🚀 Future Improvements

Potential enhancements include:

- Random Forest Regression
- XGBoost Regression
- Time Series Sales Forecasting
- Interactive Power BI Dashboard
- Streamlit Web Application
- Customer Segmentation
- Sales Forecast API
- Deployment using Flask or FastAPI

---

# 📸 Project Preview

Include screenshots of:

- Monthly Net Revenue by Region
- Average Units Sold by Product Category
- Revenue Distribution by Region
- Correlation Heatmap
- Revenue by Product Category
- Actual vs Predicted Net Revenue

Save images in the `charts/` or `images/` folder and reference them here.

---

# 👨‍💻 Author

**Carlos Mwalim**

**Aspiring Data Analyst | Business Intelligence Enthusiast**

### Skills Demonstrated

- Python
- Data Cleaning
- Feature Engineering
- Exploratory Data Analysis (EDA)
- Data Visualization
- Machine Learning
- Linear Regression
- Business Intelligence
- Statistical Analysis

---

## ⭐ If you found this project useful, feel free to star the repository and share your feedback!
