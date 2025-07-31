# Task 5 -Credit Card Fraud Detection

## Overview
The dataset was provided by CodSoft i.e. the kaggle dataset. This project builds the machine learning models to detect the fraud credit card transactions. It includes data analysis, data preprocessing, feature engineering, handling class imbalance with techniques like SMOTE and TOMEK links, along with SMOTEENN and model training models like Logistic Regression, Random Forest and XgBoost.

## Features
- Data analysis.
- Feature engineering i.e. adding new feature on the column.
- Standaradization of the columns.
- Handling the imbalanced datasets with oversampling and undersampling method along with combined as well.
- Training classification models.
- Evaluation of model using metrics like precision, recall and F1-score through classification_report and classification_matrix.

## Installation
1. Clone the repository.
2. Install requirements.txt
2. Download the datasets and then run the program as this is modular approach.

## Process of building the model
### Data analysis: 
The Kaggle dataset of the **Credit Card Fraud Detection**  was loaded and viewed using various plot to visualize the imabalances of the results i.e. fraud and non fraud, and heatmap to show the correlationship between the features.

### Feature Engineering:
New feature was added so as to see the hidden relationship and to make the model more accurate i.e. increasing recall score as this is fraud detection model.

### Scaling of the datasets:
While all other columns were PCA transformed, some columns are scaled using StandardScaler.

### Modelling
As the dataset is so imbalanced, I used SMOTE (oversampling), undersampling , SMOTEToken, SOMTEENN to make this dataset more balanced.
Then various modelling techniques are used in these transformed datasets and the metrics are compared.
Used GridSearchCv to hypertune the model and make the model more accurate to detect fraud.
XGBoost is also used to compare the evaluated metrics with the Logistic Regression and Random Forest Classifier.

### Evaluation of the model
- Classification_report and Classification_matrix is used.
- Recall score is highest in GridSearchCv i.e. 80% with feature engineering ans without feature engineering is 81%.

## Result
As the model gave the best result in GridSearchCV, so using Random Forest Regressor with hyperparameter tuning, feature engineering, SMOTEENN, SMOTEToken is the best.

## Author 
- **Nirika Lamichhane**
- **Email: nirikalamichhane12@gmail.com**