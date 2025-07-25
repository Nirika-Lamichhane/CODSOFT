# Movie Ratung Prediction Project

## Project overview
The Movie Rating Prediction project aims to build machine learning models that accurately predict the ratings of movies based on multiple features such as genre, director, and actors. By analyzing historical movie data, this project provides insights into the factors influencing movie ratings and uses various regression techniques to estimate movie ratings effectively.
This project is done in the modular approach where each folder has the specific purpose as analysis,cleaning, feature enginnerng ,modelling

## Dataset
CodSoft provided me with the kaggle datasets which includes various features among which the model is prepared using Genre, Director and Actors (i.e. all categorical) and made prediction for the Ratings of movie (i.e. numerical).

## Process on building this model
### Data analysis 

### Data processing 
Missing values of the datasets are being handled and filled with the NaN values as putting mean or any statistical values can change the overall value of this categorical features for predicting numerical target (Rating).

### Feature Engineering 
Encoding of the categorical features is done so as the various ml algorithm can works upon. 
Here various techniques are used as: 
For Genre column : MultiLabelBinarizer
For Director column : One Hot Encoding, Frequency Encoding
For Actors column : Binary encoding

### Modelling approaches
This project is done using various approaches to check and compare their results as:
**Linear Rregression**
**Random Forest Regression**
**Gradient Boosting Regressor**
**XGBoost Regressor**

### Used Hyperparamter Tuning 
Did this using the "GridSearchCV" to tune the model parameters and check the results as how this varies the final data.
Used parameters are: 
- Number of estimators (`n_estimators`)
- Maximum tree depth (`max_depth`)
- Learning rate (for boosting models)
- Minimum samples split

### Evaluation metrics
The prepared model was evaluated using different metrics as: 
- **Mean Absolute Error (MAE)**
- **Mean Squared Error (MSE)**
- **Root Mean Squared Error (RMSE)**
- **R² Score**

### Future Work
- Incorporate additional features for prediction.
- Explore deep learning techniques for potentially improved prediction.

## Prerequisites
- Python 3.7 or higher
- Install required packages as in requirements.txt

## Author 
- **Nirika Lamichhane**
- **Email: nirikalamichhane12@gmail.com**
