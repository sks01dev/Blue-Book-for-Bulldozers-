# 🏗️ Bulldozer Price Prediction – Kaggle Blue Book for Bulldozers

[![Python](https://img.shields.io/badge/Python-3.10-blue)](https://www.python.org/)
[![Pandas](https://img.shields.io/badge/Pandas-1.5-green)](https://pandas.pydata.org/)
[![Matplotlib](https://img.shields.io/badge/Matplotlib-3.8-yellow)](https://matplotlib.org/)
[![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-1.3-orange)](https://scikit-learn.org/)

This repository contains my solution to the **Kaggle Competition – Blue Book for Bulldozers**, where the task is to **predict the auction sale price** of heavy equipment based on historical sales data, usage, and configuration.

---

## 📘 Project Overview

The **goal** is to build a machine learning model that can estimate the **sale price of bulldozers at auction**.  

Competition details:  
- **Host**: [Kaggle – Blue Book for Bulldozers](https://www.kaggle.com/competitions/bluebook-for-bulldozers)  
- **Evaluation Metric**: RMSLE (Root Mean Squared Logarithmic Error)  
- **Dataset**: Auction results with fields like equipment type, usage hours, year of manufacture, and sale date.  

---

## 🔧 Steps Implemented

1. **Data Import & Exploration**
   - Loaded training and validation datasets using **Pandas**.
   - Explored dataset with `.info()`, `.head()`, and `.isna().sum()`.
   - Plotted sale price distributions and scatter plots for time trends.

2. **Feature Engineering**
   - Converted `saledate` column into **datetime features** (`year`, `month`, `day`, `dayofweek`, etc.).
   - Created a temporary working dataframe `df_tmp` to process engineered features.
   - Handled missing values and irrelevant columns.

3. **Data Visualization**
   - Distribution plots for `SalePrice`.
   - Scatter plots of `saledate` vs. `SalePrice`.

4. **Modeling**
   - Prepared feature matrix `X` and target variable `y`.
   - Applied **Scikit-Learn models** to predict prices.
   - Evaluated results using **RMSLE** metric.

---

## 🛠️ Technologies Used

- **Python 3.10**
- **Pandas** – data manipulation  
- **Matplotlib / Seaborn** – visualization  
- **Scikit-Learn** – ML modeling & evaluation  

---

## 📌 Key Learnings

- Feature engineering from **date-time data** is crucial in time-sensitive price prediction.  
- **Random Forest Regressor** provides a strong baseline for tabular datasets.  
---

## 🔗 Resources

- 📘 [Kaggle Competition – Blue Book for Bulldozers](https://www.kaggle.com/competitions/bluebook-for-bulldozers)  
- 📊 [Scikit-Learn Documentation](https://scikit-learn.org/stable/)  
- 🐼 [Pandas Documentation](https://pandas.pydata.org/)  

