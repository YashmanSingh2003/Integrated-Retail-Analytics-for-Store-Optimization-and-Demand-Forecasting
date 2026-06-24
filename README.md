# 🛒 Integrated Retail Analytics for Store Optimization and Demand Forecasting

## 📌 Project Overview

This project applies data analytics and machine learning techniques to optimize retail operations through demand forecasting, anomaly detection, store segmentation, and sales pattern analysis.

Using historical sales data, store information, and external economic indicators, the project provides actionable insights that can help retailers improve inventory management, marketing effectiveness, and overall store performance.

---

## 🎯 Project Objectives

* Forecast weekly sales demand across stores and departments.
* Detect anomalies and unusual sales patterns.
* Analyze seasonal and holiday-driven sales behavior.
* Evaluate the impact of external factors such as CPI, Fuel Price, and Unemployment.
* Segment stores based on operational and sales characteristics.
* Identify potential cross-selling opportunities through department co-occurrence analysis.
* Develop data-driven business recommendations for inventory and marketing optimization.

---

## 📂 Dataset Description

The project uses three datasets:

### 1. Sales Dataset

Contains weekly sales information for each store and department.

**Key Features**

* Store
* Dept
* Date
* Weekly_Sales
* IsHoliday

### 2. Stores Dataset

Contains store-level attributes.

**Key Features**

* Store
* Type
* Size

### 3. Features Dataset

Contains external factors that may influence sales.

**Key Features**

* Temperature
* Fuel_Price
* CPI
* Unemployment
* MarkDown1 – MarkDown5
* IsHoliday

---

## ⚙️ Project Workflow

### Data Preprocessing

* Data loading and inspection
* Missing value treatment
* Dataset integration
* Date conversion and sorting
* Feature encoding
* Feature scaling

### Exploratory Data Analysis

* Sales distribution analysis
* Anomaly detection using IQR
* Time-series trend analysis
* Holiday impact analysis
* Correlation analysis

### Feature Engineering

Created:

* Year
* Month
* Week Number
* 4-Week Rolling Average Sales

### Machine Learning Models

* Linear Regression (Baseline Model)
* Random Forest Regressor

### Store Segmentation

* K-Means Clustering
* PCA Visualization
* Silhouette Score Evaluation

### Market Basket-Style Analysis

* Department sales co-occurrence analysis
* Cross-selling opportunity identification

---

## 📊 Model Performance

### Linear Regression

| Metric   | Value         |
| -------- | ------------- |
| MAE      | 1,693.66      |
| MSE      | 24,388,776.07 |
| R² Score | 0.9532        |

### Random Forest Regressor

| Metric   | Value         |
| -------- | ------------- |
| MAE      | 1,446.92      |
| MSE      | 14,299,629.13 |
| R² Score | 0.9726        |

✅ Random Forest achieved the best performance and was selected as the preferred forecasting model.

---

## 🔍 Key Findings

### Demand Forecasting

* Historical sales trends strongly influence future demand.
* Random Forest effectively captures complex sales patterns.

### Holiday Impact

* Holiday periods significantly affect weekly sales.
* Seasonal demand fluctuations were clearly identified.

### Store Segmentation

Three distinct store segments were identified:

* High-performing stores
* Medium-performing stores
* Lower-performing stores

Segmentation quality evaluation:

| Metric           | Value  |
| ---------------- | ------ |
| Silhouette Score | 0.3345 |
| Inertia          | 107.18 |

### Promotional Analysis

* MarkDown variables were among the most influential sales drivers.
* Promotional activities have a measurable impact on demand.

### Market Basket Insights

* Several departments exhibit strong sales co-occurrence patterns.
* Opportunities exist for cross-selling and bundled promotions.

---

## 💡 Business Recommendations

### Inventory Optimization

* Use demand forecasts for inventory planning.
* Increase stock levels during predicted peak-demand periods.

### Marketing Strategy

* Apply segment-specific promotional campaigns.
* Optimize markdown schedules around holidays and seasonal demand.

### Store Management

* Tailor operational strategies based on store segment characteristics.
* Focus improvement initiatives on lower-performing stores.

### Cross-Selling Opportunities

* Bundle frequently associated departments.
* Improve store layout and product placement.

---

## 🛠️ Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-Learn

---

## 📈 Future Improvements

* Implement XGBoost and LightGBM models.
* Use time-series cross-validation.
* Incorporate weather and demographic datasets.
* Perform true market basket analysis using transaction-level data.
* Deploy forecasting models through an interactive dashboard.

---

## 📚 Conclusion

This project demonstrates how machine learning and data analytics can transform retail data into actionable business insights. Through forecasting, segmentation, anomaly detection, and sales pattern analysis, the project provides a framework for improving inventory management, marketing effectiveness, and strategic decision-making in a retail environment.

