# Predictive Modeling with Linear Regression - ShowTime
## 📌 Project Overview

In the competitive streaming industry, understanding what drives first-day content performance is crucial for optimizing marketing strategies and release planning. This project analyzes the key factors influencing first-day content views on the ShowTime platform using statistical analysis and predictive modeling.

Using Exploratory Data Analysis (EDA), feature engineering, and multiple linear regression, the study identifies how marketing efforts, platform traffic, release timing, and external events affect content performance.

The goal is to develop a data-driven model capable of predicting first-day viewership and providing actionable business insights.

## 🎯 Objectives

The main objectives of this project are:
- Analyze the factors influencing first-day content views.
- Explore relationships between marketing metrics and content performance.
- Develop a multiple linear regression model to predict content views.
- Evaluate model performance using statistical metrics.
- Generate actionable insights for content release strategy and marketing decisions.

## 📊 Dataset Description

The dataset contains 1000 observations, where each row represents a content release on the ShowTime platform.

### Target Variable
- views_content → Number of views a piece of content received on its first day of release.

### Numerical Variables
- visitors → Platform visitors during the release period
- ad_impressions → Number of advertising impressions
- views_trailer → Trailer views before release

### Categorical Variables
- genre → Content genre (Drama, Comedy, Action, etc.)
- dayofweek → Day of release
- season → Season of release

### Binary Variable
- major_sports_event → Whether a major sports event was occurring during the release (0 = No, 1 = Yes)

## 🔍 Exploratory Data Analysis (EDA)
Exploratory analysis was conducted to understand dataset characteristics and identify patternsin content performance.

### Key EDA Insights
- Trailer views show a strong positive correlation with first-day content views.
- Platform visitors have a moderate influence on content performance
- Advertising impressions show a minimal direct impact.
- Major sports events negatively affect viewership.
- Content views show a right-skewed distribution, indicating a few high performing titles.

## 🔍 Exploratory Data Analysis (EDA)

Before building the regression model, the dataset underwent preprocessing steps:

### Outlier Detection

Outliers were detected using boxplots and the IQR method.

### Feature Engineering

Categorical variables were converted into numerical from using one-hot encoding.

## 🤖 Model Building

A Multiple Linear Regresion model was developed to predict first-day content views.

Steps Included:
- Defining independent and dependent variables.
- Splitting data into training (80%) and testing (20%) sets.
- Adding an intercept term.
- Training the regression model using Ordinary Least Squares (OLS).

## 📈 Model Performance

The regression model achieved strong predictive performance.
| Metric | Value |
|--------|-------|
| R² | ~0.60|
| MAE | ~0.049 |
| MSE | ~0.00399 |
| RMSE | ~0.063 |

### Interpretation:
- The model explains about 60% of the variation in first-day content views.
- Prediction errors are relatively small, averaging around 50,000 views.
- The model generalizes well to unseen data without overfitting.

## 💡 Key Insights
### 1️⃣ Trailer Engagement Drives Performance

Trailer views show the strongest positive relationship with first-day views, indicating that pre-release engagement is critical.

### 2️⃣ Platform Traffic Matters

Higher visitor traffic significantly increases content consumption.

### 3️⃣ Sports Events Reduce Viewership

Major sports events divert audience attention, negatively affecting launch-day performance.

### 4️⃣ Release Timing Influences Performance

Certain days of the week and seasons show slightly higher average viewership.

### 5️⃣ Advertising Volume Alone Is Not Enough

Ad impressions are not statistically significant when other variables are considered.

## 📌 Business Recommendations

Based on the analysis:
- Focus marketing efforts on increasing trailer engagement.
- Avoid releasing major content during large sports events.
- Schedule releases during high-traffic periods.
- Prioritize engagement-driven marketing strategies over simply increasing ad impressions.

## 🛠 Tools and Technologies
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Statsmodels
- Jupyter Notebook

## 📄 Project Report

The full report can be found here:

report/Predictive Modeling with Linear Regression ShowTime.pdf

## 👩‍💻 Author

Arhana Sen Chowdhury

Aspiring Data Analyst | Data Science Enthusiast

This project demonstrates the application of statistical modeling and data analysis techniques to real-world business problems.
