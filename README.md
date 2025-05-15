Absolutely! Here's an updated and improved version of your **README file**, fully aligned with your **final-year project**, including your actual models used (XGBoost, CatBoost, etc.), SHAP interpretability, and Power BI dashboard:

---

# 🍽️ Demand Forecasting for a Sri Lankan Restaurant's Uber Eats Sales using Machine Learning

## 📌 Project Overview

This project aims to forecast **daily Uber Eats sales** for a **Sri Lankan restaurant** by integrating **non-linear external factors** such as **weather conditions** and **inflation trends**. Traditional linear forecasting approaches fail to capture the complex relationships between these variables and sales. Therefore, this project leverages **ensemble machine learning models** and explainable AI to build a more robust, data-driven forecasting solution.

🔹 **Why It Matters?**

* Enables **restaurant managers** to make better **inventory, pricing, and staffing** decisions.
* Minimizes **waste and overstocking** by anticipating demand fluctuations.
* Adjusts predictions based on **economic volatility** and **weather changes**—essential for emerging markets like Sri Lanka.

---

## 🎯 Project Objectives

✅ **Build a Sales Forecasting Model**
Integrate Uber Eats transactional data with weather and inflation variables for precise daily demand prediction.

✅ **Handle Non-Linear Drivers of Demand**
Use machine learning algorithms that are better suited for capturing interactions between variables (e.g., rain × weekend, inflation × promotion).

✅ **Generate Actionable Insights for Businesses**
Develop a **Power BI dashboard** for decision-makers to monitor sales trends, feature impacts, and economic conditions.

✅ **Ensure Interpretability and Transparency**
Apply **SHAP** (SHapley Additive Explanations) to interpret the influence of each variable on sales predictions.

---

## 📊 Dataset Overview

The project combines **multiple datasets** from **2021 to 2024**, including:

* 🛵 **Uber Eats Sales Data**: Order-level records with revenue, order channel, delivery mode, and customer tier.
* 🌧 **Weather Data**: Daily rainfall, temperature, and weather conditions (sourced via meteorological APIs).
* 💸 **Inflation Data**: CPI-based inflation index rebased to 2021 baseline for comparability.

### 🔧 Preprocessing Highlights

✔️ Cleaned missing values and handled structured gaps using context-aware imputation.
✔️ Rebased CPI index to 2021 and created a smoothed YoY inflation rate.
✔️ Engineered **interaction terms**: `rain_x_weekend`, `inflation_x_promo`.
✔️ Normalized numerical features and applied **one-hot encoding** to categorical variables.

---

## 🏗 Methodology

### 1️⃣ Data Preparation

* Combined Uber Eats, CPI, and weather datasets into a unified DataFrame.
* Performed **backward fill** and logical imputation.
* Created lag/rolling features and calculated average weather metrics.

### 2️⃣ Exploratory Data Analysis (EDA)

* Visualized trends in sales, rainfall, inflation, and day-of-week patterns.
* Identified non-linear behaviours and periods of high economic volatility.
* Correlated weather types and macroeconomic events with demand spikes and drops.

### 3️⃣ Model Development

#### 📌 Models Used:

* **Linear Regression** (baseline)
* **Random Forest Regressor** 🌲
* **XGBoost Regressor** ⚡️ *(Best performing model — RMSE: 788.77, R²: 0.3797)*
* **CatBoost Regressor** 🐱 *(Efficient with categorical features)*

#### 📊 Evaluation Metrics:

* **RMSE** – Root Mean Squared Error
* **MAE** – Mean Absolute Error
* **R² Score** – Coefficient of Determination

### 4️⃣ Explainability (SHAP)

* Used SHAP to interpret model predictions and identify top contributing features:

  * `rain_sum`, `YoY_inflation_rate_smoothed`, `weekend`, and `rain_x_weekend`.

---

## 📈 Results & Insights

* 📊 **XGBoost** outperformed other models in all evaluation metrics.
* 🔍 SHAP revealed rainfall and inflation as the most critical predictors.
* 📉 Inflation had a **negative impact** on sales during economic crises, while **rain increased orders**, especially on weekends.
* 📈 Interaction terms boosted model accuracy and offered behavioural interpretability.

---

## 📊 Interactive Dashboard (Power BI)

An interactive **Power BI dashboard** was built for non-technical stakeholders:

* 🔹 **Page 1** – Sales performance: Predicted vs Actual, Order Channels, Monthly Forecast
* 🔹 **Page 2** – Weather & Inflation Impact: Rainfall trends, CPI vs Sales
* 🔹 **Page 3** – Customer Segments: Uber One, Dine-in vs Delivery, Platform breakdown

---

## 🚀 Future Work

* Integrate **real-time data feeds** for weather and inflation forecasting.
* Develop **segment-specific models** for Uber One members and promo users.
* Explore **LSTM models** for capturing long-term temporal dependencies.
* Expand SHAP integration into the dashboard for daily interpretability.

---

## 📚 Technologies Used

* 🐍 **Python (Pandas, Scikit-learn, XGBoost, CatBoost, SHAP)**
* 📊 **Power BI** for dashboard development
* 📈 **Matplotlib & Seaborn** for EDA
* 💾 **Google Colab** & **Gemini AI** for iterative development and code generation

---

Would you like this converted into a GitHub README markdown file (`README.md`) or embedded into your report as a project summary?
