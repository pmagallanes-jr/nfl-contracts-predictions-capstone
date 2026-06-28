# NFL Contracts Prediction Capstone

## Overview

This repository contains the notebooks for my capstone project exploring whether historical NFL player performance can be used to predict future contract values for offensive skill positions.

The project focuses on quarterbacks (QB), running backs (RB), wide receivers (WR), and tight ends (TE), using player performance data from the 2000–2025 NFL seasons combined with contract information to develop predictive machine learning models.

The work is divided into two notebooks:

1. **NFL Initial Data Analysis**
   - Data collection
   - Cleaning
   - Exploratory Data Analysis (EDA)
   - Feature engineering
   - Creation of modeling datasets

2. **NFL Contracts Predictions Analysis**
   - Model development
   - Baseline model comparisons
   - Feature engineering experiments
   - Hyperparameter tuning
   - Feature importance analysis
   - Final model evaluation

---

# Research Question

**Can historical on-field performance reliably predict the value of an NFL offensive player's next contract?**

This project investigates how cumulative career production, playoff performance, and efficiency metrics influence player contract values while comparing multiple machine learning algorithms to determine which models best estimate Average Annual Salary (APY).

---

# Repository Contents

| Notebook | Description |
|-----------|-------------|
| **NFL_Initial_Data_Analysis.ipynb** | Imports NFL data, cleans and prepares datasets, engineers features, and performs exploratory data analysis. |
| **NFL_Contracts_Predictions_Analysis.ipynb** | Builds predictive models, compares algorithms, performs feature selection, tunes hyperparameters, and evaluates model performance. |

---

# Notebook Links

## 1. NFL Initial Data Analysis

This notebook covers:

- Importing NFLVerse player, team, schedule, and contract data
- Data cleaning and preprocessing
- Missing value handling
- Contract filtering
- Exploratory Data Analysis
- Creation of cumulative player statistics
- Initial feature engineering

**Notebook:**

[NFL Initial Data Analysis](https://github.com/pmagallanes-jr/nfl-contracts-predictions-capstone/blob/main/NFL_Initial_Data_Analysis.ipynb)

---

## 2. NFL Contracts Predictions Analysis

This notebook focuses on:

- Baseline Linear Regression models
- Position-specific modeling (QB, RB, WR, TE)
- Comparison of multiple regression algorithms
- Feature importance extraction
- Consensus feature ranking
- Hyperparameter tuning
- Final model evaluation

**Notebook:**

[NFL_Contracts_Predictions_Analysis](https://github.com/pmagallanes-jr/nfl-contracts-predictions-capstone/blob/main/NFL_Contracts_Predictions_Analysis.ipynb)

---

# Machine Learning Models

The following regression models were evaluated throughout the project:

- Linear Regression
- Random Forest Regressor
- Extra Trees Regressor
- Gradient Boosting Regressor
- XGBoost Regressor
- CatBoost Regressor

Model performance was evaluated using:

- Root Mean Squared Error (RMSE)
- Mean Absolute Error (MAE)
- R² Score
- Cross-validation

---

# Feature Engineering

Several feature sets were explored throughout the modeling process, including:

- Career cumulative statistics
- Regular season and playoff production splits
- Efficiency metrics
- Position-specific statistics
- Draft information
- Player demographics

Feature importance was compared across multiple models to identify the most consistently predictive variables.

---

# Summary of Findings

Key observations from this project include:

- Tree-based and ensemble models consistently outperformed the Linear Regression baseline.
- CatBoost, XGBoost, and Random Forest provided the strongest predictive performance across multiple experiments.
- Career cumulative production remained one of the strongest predictors of future contract value.
- Incorporating additional contextual features such as playoff production and efficiency metrics further improved predictive performance over cumulative statistics alone.
- Consensus feature ranking across multiple models provided a robust approach for identifying the most influential variables while reducing redundant features.

Overall, the results suggest that historical player performance can provide meaningful insight into future NFL contract values, although the importance of individual statistics varies by position and model.

---

# Data Source

All football data was obtained using the **NFLVerse** project.

Contract information and player statistics were collected from publicly available NFLVerse datasets.

---

# Future Improvements

Potential future work includes:

- Incorporating advanced player tracking metrics
- Including team salary cap and roster context
- Predicting total contract value and guarantees in addition to APY
- Expanding the analysis to defensive and special teams players
- Exploring deep learning and stacking ensemble approaches

---

# Author

**Pablo Magallanes Jr.**

UC Berkeley Professional Certificate in Machine Learning & Artificial Intelligence

Capstone Project
