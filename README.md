Flight Fare Prediction using Machine Learning
Project Overview

This project aims to predict flight ticket prices based on various factors such as airline, source, destination, duration, total stops, and journey timing. The objective is to help customers estimate future flight fares and make informed travel decisions.

Problem Statement
Task 1

Perform comprehensive data analysis on the flight fare dataset.

Task 2

Build a machine learning model capable of predicting flight ticket prices accurately.

Dataset Features

The dataset contains information such as:

Airline
Source
Destination
Route
Total Stops
Journey Date
Departure Time
Arrival Time
Duration
Additional Information
Price (Target Variable)
Technologies Used
Python
Pandas
NumPy
Matplotlib
Seaborn
Scikit-learn
Project Workflow
1. Data Preprocessing
Handling missing values
Feature extraction from date and time columns
Data cleaning
One Hot Encoding of categorical variables
2. Exploratory Data Analysis (EDA)
Airline-wise fare analysis
Source and destination analysis
Duration vs Price analysis
Stops vs Price analysis
Correlation analysis
3. Feature Engineering

Created meaningful features such as:

Journey Day
Journey Month
Departure Hour
Departure Minute
Arrival Hour
Arrival Minute
Duration Hours
Duration Minutes
4. Model Building

The following regression models were implemented:

Linear Regression
Decision Tree Regressor
Random Forest Regressor
5. Hyperparameter Tuning

RandomizedSearchCV was used to optimize Random Forest parameters.

Model Evaluation

Evaluation Metrics:

Mean Squared Error (MSE)
Mean Absolute Error (MAE)
R² Score
Random Forest Performance
Metric	Value
MSE	4028216
MAE	1203
R² Score	0.8069

Random Forest achieved the best performance among all tested models.

Key Findings
Flight duration significantly impacts ticket price.
Flights with more stops generally have higher fares.
Airline choice plays a major role in pricing.
Random Forest effectively captured nonlinear relationships in the dataset.
Challenges Faced
Handling categorical features
Feature extraction from datetime columns
Managing nonlinear relationships
Preventing overfitting
Evaluating model performance on unseen data
Conclusion

The Random Forest Regressor provided the best predictive performance with an R² score of approximately 0.81. The model successfully learned pricing patterns from historical flight data and can be used to estimate future flight fares.

Future Improvements
Implement Gradient Boosting Regressor
Implement XGBoost Regressor
Deploy using Streamlit
Create an interactive prediction dashboard
