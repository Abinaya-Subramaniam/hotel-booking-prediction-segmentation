# 🏨 Hotel Booking Analysis and Prediction

This project explores hotel booking data to **predict cancellations**, **understand customer behavior**, and **segment guests** for personalized marketing. The analysis covers Exploratory Data Analysis (EDA), Predictive Modeling, Hypothesis Testing, Revenue Loss Estimation, and Customer Segmentation.

## 📌 Objectives

- Identify patterns and factors influencing cancellations and no-shows
- Predict reservation outcomes (Check-in, Canceled, No-show) using ML models
- Segment customers using clustering to support targeted strategies
- Interpret model predictions for actionable insights

---

## 🧠 Methods & Workflow

### 1. Exploratory Data Analysis (EDA)

- **Data Cleaning**: Handled missing values, converted datetime fields, and dropped irrelevant columns.
- **Encoding**:
  - Ordinal: Income
  - One-Hot: Ethnicity, Hotel Type, Region, etc.
  - Binary: Promotions, Car Parking, etc.
- **Feature Engineering**: Created features like stay duration, month, and day of the week.

### 2. Hypothesis Testing

Used statistical tests like:
- Chi-Square (Categorical independence)
- ANOVA (Group differences)
- t-Test (Spending behavior)

### 3. Revenue Loss Estimation

Calculated potential revenue loss from cancellations and no-shows:


### 4. Predictive Modeling

Implemented various classification models:
- Logistic Regression
- Decision Tree, Random Forest
- XGBoost, LightGBM, CatBoost (Best Performing)

**Handling Imbalance**: Used SMOTE (Synthetic Minority Over-sampling) to balance classes.

**Evaluation Metrics**:
- Weighted F1-Score
- Confusion Matrix

### 5. Customer Segmentation

Used **K-Means Clustering** to group customers based on features like income, room rate, booking channel, etc.

- **Feature Scaling**: StandardScaler
- **Elbow Method**: Determined 4 optimal clusters
- Resulted in meaningful guest profiles for marketing insights

### 6. Model Explainability

- Employed **SHAP (SHapley Additive Explanations)** to interpret model predictions and understand feature importance.

---

## 📂 Dataset

- **Training Data**: 27,499 entries × 24 features
- **Validation Data**: 2,749 entries

Features include demographic details, booking preferences, and reservation status.

---

## 📊 Key Insights

- **Deposit Type**, **Booking Channel**, and **Promotional Use** strongly influence cancellations.
- CatBoost was the **most accurate and balanced** model across all metrics.
- Segmented guests showed distinct patterns for revenue optimization and retention.

---

