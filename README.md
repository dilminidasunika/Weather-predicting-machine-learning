### 🌦️ Weather Analysis & Maximum Temperature Prediction

📌 Project Overview

This project analyzes global weather station data and uses Machine Learning to investigate the relationship between Minimum Temperature (MinTemp) and Maximum Temperature (MaxTemp).

The main objectives of this project are:

Determine whether there is a relationship between MinTemp and MaxTemp.
Predict MaxTemp using MinTemp.
Compare the performance of Linear Regression and Random Forest Regression.
Evaluate the models using R², MAE, and RMSE.

The project follows a complete data analysis and machine learning workflow, including data loading, cleaning, exploratory data analysis, visualization, correlation analysis, model building, prediction, and evaluation.

### 🎯 Research Questions

Question 1

Is there a relationship between MinTemp and MaxTemp?

Question 2

Can MaxTemp be predicted using MinTemp?

### 📊Dataset & Data Preparation

The dataset contained 119,040 records and 31 columns. For this analysis, I focused on MinTemp and MaxTemp.

The data preparation process included:

• Checking missing values and data types

• Detecting and removing duplicate records

• Obtaining a final dataset of unique valid records


### 📈Exploratory & Statistical Analysis

I performed:

• Summary statistical analysis
• Temperature distribution visualizations
• MinTemp vs MaxTemp scatter plot
• Daily temperature range analysis
• Pearson correlation analysis

### 📊 Data Visualization

Several visualizations were created to understand the dataset:

Temperature Distributions

Histograms were created for:

Minimum Temperature
Maximum Temperature

These visualizations helped examine how temperature values were distributed.

### 🔗 Correlation Analysis

Pearson correlation was used to measure the relationship between MinTemp and MaxTemp.

Result
Pearson Correlation = 0.9252

This indicates a very strong positive relationship between the two variables.

In general:

When MinTemp increases, MaxTemp also tends to increase.

### 🤖 Machine Learning

Two regression models were developed and compared.

## Model 1 — Linear Regression

Linear Regression was selected because the scatter plot and correlation analysis indicated a strong linear relationship.

## Model 2 — Random Forest Regression

A Random Forest Regressor was also trained using:

The Random Forest model uses multiple decision trees and combines their predictions.

It was included to determine whether a more complex model could improve prediction performance compared with Linear Regression

### 🧪 Train/Test Split

The dataset was divided into:

80% training data
20% testing data

### 📏 Model Evaluation

The models were evaluated using three metrics:

R² — Coefficient of Determination

Measures how much of the variation in the target variable is explained by the model.

Higher is better.

MAE — Mean Absolute Error

Measures the average absolute difference between actual and predicted values.

Lower is better.

RMSE — Root Mean Squared Error

Measures prediction error while giving more weight to larger errors.

Lower is better.

###📌 Final Results

Research Question 1

Is there a relationship between MinTemp and MaxTemp?

✅ Yes.

The Pearson correlation coefficient was:

r = 0.9252

This represents a very strong positive relationship.

Research Question 2

Can MaxTemp be predicted using MinTemp?

✅ Yes.

The recommended model was Linear Regression.

MaxTemp = 11.62 + 1.04 × MinTemp

Performance:

R²   = 0.8499
MAE  = 5.7483°C
RMSE = 6.9901°C

The model explains approximately 84.99% of the variation in MaxTemp.

## 🚀 Machine Learning Workflow

```text
Load Dataset
      ↓
Select Required Columns
      ↓
Check Missing Values
      ↓
Check Data Types
      ↓
Remove Invalid Records
      ↓
Remove Duplicates
      ↓
Exploratory Data Analysis
      ↓
Data Visualization
      ↓
Correlation Analysis
      ↓
Train/Test Split
      ↓
Build Linear Regression
      ↓
Build Random Forest
      ↓
Generate Predictions
      ↓
Evaluate Models
      ↓
Compare Models
      ↓
Select Best Model
```

### 💡Key Learnings

This project provided practical experience with:

Data cleaning and preprocessing

Handling invalid and duplicate records

Exploratory Data Analysis

Statistical analysis

Correlation analysis

Data visualization

Feature and target selection

Train/test splitting

Regression algorithms

Machine Learning model evaluation

Comparing simple and complex models

Interpreting R², MAE and RMSE

Drawing conclusions from model results
