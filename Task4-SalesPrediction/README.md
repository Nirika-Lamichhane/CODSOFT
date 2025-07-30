# Task 3: Sales Prediction Using Regression Models

##  Project Overview
This project focuses on predicting **sales** based on advertising expenses in **TV**, **Radio**, and **Newspaper** channels.

To evaluate and compare model performance, the following regression models were used:
- Linear Regression
- Ridge Regression
- Huber Regression

## Highlights
- Performed **cross-validation** due to the small dataset size (200 rows), instead of a traditional train-test split.
- Used **Linear Regression** as the base model with CV, then analyzed residuals for potential outliers.
- Evaluated model performance using **RMSE** and **R² Score**.
- Found that **all three models performed similarly**, indicating that the dataset is clean and outliers have minimal impact.
- Final conclusion: **Linear Regression** is sufficient due to clean data and stable performance across models.

## How to Run

1. **Clone the repository**  
2. **Install required dependencies**
3. **run the notebook**

## Process of Building the Model

### Data Analysis
- The dataset (provided by CodSoft) had **no missing values** and appeared clean.
- Basic exploratory analysis showed that most features (TV, Radio, Newspaper) were **numerically continuous**.
- Some correlation observed between features and the target variable **Sales**.

### Data Cleaning
- **Outliers and skewness** were detected, especially in the **Newspaper** column.
- Applied the **IQR method** to detect and handle outliers.
- Instead of removing them, **capping** was performed to avoid data loss.

### Feature Scaling
- As all features are **numerical**, no categorical encoding was needed.
- Both **StandardScaler** and **MinMaxScaler** were experimented with.
- Final decision: **StandardScaler** was used since it worked consistently better across all models.

### Modeling
- Trained a **Linear Regression** model with **Cross-Validation (CV)** instead of train-test split due to the small dataset (only 200 rows).
- Plotted **standardized residuals** to check for the presence of **outliers**.
- Applied:
  - **Ridge Regression** to reduce overfitting and check regularization effect.
  - **Huber Regression** for robust regression in case of hidden residuals outliers.
- Compared all models using **RMSE** and **R² Score** metrics.

### Final Model Selection
- All models gave **similar performance metrics**, indicating:
  - The data was clean.
  - Outliers did not significantly affect predictions.
- Final choice: **Linear Regression** was selected for its simplicity and effective performance.

## Author 
- **Nirika Lamichhane**
- **Email: nirikalamichhane12@gmail.com**
