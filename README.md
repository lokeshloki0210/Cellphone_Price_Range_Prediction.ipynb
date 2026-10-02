# 📱 Mobile Phone Price Range Prediction

## 📌 Project Overview

This project analyzes mobile phone specifications and uses Machine Learning classification algorithms to predict the **price range** of a mobile phone.

The prediction is based on specifications such as battery power, RAM, internal memory, camera specifications, screen dimensions, connectivity features, processor cores, and other mobile characteristics.

The target variable `price_range` represents four price categories:

- `0` – Low Cost
- `1` – Medium Cost
- `2` – High Cost
- `3` – Very High Cost

## 🎯 Business Problem

A new mobile company wants to understand how different mobile specifications are associated with different price ranges.

Instead of predicting the exact selling price, this project builds a classification model that predicts the appropriate **price category** for a mobile phone.

The analysis also helps identify which mobile specifications are important for positioning phones into different market segments.

## 📊 Data Analysis

The project performs:

- Dataset structure and dimension analysis
- Data type analysis
- Missing-value analysis
- Duplicate-value analysis
- Statistical analysis
- Price-range distribution analysis
- Feature correlation analysis
- Relationship between specifications and price range
- Outlier analysis
- Feature importance analysis

## 🛠️ Data Preparation

The dataset was checked for missing values and duplicate records before model development.

The target variable is:

`price_range`

The remaining mobile phone specifications are used as input features.

The dataset is divided into training and testing sets using an **80:20 split** with stratification to maintain the distribution of price-range classes.

Feature scaling using `StandardScaler` is applied through pipelines for models that are sensitive to feature scaling, including:

- Logistic Regression
- K-Nearest Neighbors
- Support Vector Machine

## 🤖 Machine Learning Models

The following classification algorithms are trained and compared:

1. Logistic Regression
2. Decision Tree
3. Random Forest
4. Gradient Boosting
5. Extra Trees
6. K-Nearest Neighbors (KNN)
7. Support Vector Machine (SVM)

### Evaluation Metrics

The models are evaluated using:

- Accuracy
- Precision
- Recall
- F1 Score
- Confusion Matrix
- Classification Report

## 🔧 Hyperparameter Tuning

GridSearchCV is used to tune the Logistic Regression model.

The tuning process uses **5-fold cross-validation** and searches for the best value of the regularization parameter `C`.

## ⭐ Feature Importance

Feature importance is analyzed using:

- Random Forest feature importance
- Logistic Regression coefficients

This helps identify the mobile specifications that contribute most to price-range prediction.

## 🔮 Price Range Prediction

A prediction function is implemented to accept mobile phone specifications and predict the corresponding price category.

Example output categories:

```text
0 → Low Cost
1 → Medium Cost
2 → High Cost
3 → Very High Cost
