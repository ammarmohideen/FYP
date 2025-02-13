# 🍽️ Demand Forecasting for a Sri Lankan Restaurant's Uber Eats Sales using Machine Learning

## 📌 Project Overview
This project focuses on **predicting Uber Eats sales** for a **Sri Lankan restaurant** by analyzing **non-linear factors** such as **weather, inflation, and economic trends**. Traditional forecasting methods struggle to capture these relationships, so **machine learning models** (Random Forest, Gradient Boosting, and RNNs) are implemented for improved accuracy.

🔹 **Why It Matters?**
- Helps **restaurant owners** optimize **inventory, staffing, and pricing**.
- Reduces **food waste** by predicting demand more accurately.
- Adapts to **local economic and weather conditions**, unlike generic forecasting models.

---

## 🎯 Objectives
✅ **Develop a Forecasting Model** - Incorporate weather patterns, inflation, and economic trends.  
✅ **Improve Accuracy** - Use **machine learning models** that handle **non-linear data relationships**.  
✅ **Provide Actionable Insights** - Help small restaurants optimize costs and operations.  
✅ **Handle Data Limitations** - Optimize forecasting with limited datasets from Uber Eats.  

---

## 📊 Dataset
This project integrates **multiple datasets** from **2021 to 2024**, including:
- **Uber Eats Sales Data** (order details, delivery status, revenue).
- **Weather Data** (temperature, rainfall intensity).
- **Inflation Data** (CPI index adjustments).

### **Preprocessing Steps:**
✔️ Merged **multiple years of Uber Eats sales data**.  
✔️ Cleaned **missing values** and **handled duplicates**.  
✔️ Feature Engineered **rain intensity, average temperature, and adjusted CPI index**.  
✔️ Standardized **date formats** for seamless integration.  

---

## 🏗 Methodology

### **1️⃣ Data Preprocessing**
- Consolidated **Uber Eats sales, weather, and inflation** data.
- Removed **duplicate records** and **irrelevant columns**.
- **Rebased the CPI Index** (2021 = 100) to align inflation data.
- Engineered new **rain intensity and average temperature features**.

### **2️⃣ Exploratory Data Analysis (EDA)**
- **Visualized trends** in sales, weather, and inflation.
- **Identified correlations** between key factors.
- Generated **heatmaps** to study relationships.

### **3️⃣ Model Development**
- **Baseline Model**: Linear Regression.
- **Machine Learning Models**:
  - **Random Forest** 🌲 - Captures complex relationships.
  - **Gradient Boosting** 🚀 - Optimizes predictions.
  - **Recurrent Neural Networks (RNNs)** 🧠 - Handles time-series forecasting.

### **4️⃣ Model Evaluation**
- Used **RMSE, MAE, and R² Score** for performance comparison.
- Conducted **hyperparameter tuning** for model optimization.

---
