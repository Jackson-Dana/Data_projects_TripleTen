# Sprint 17 Project - Predicting Customer Churn

This is the 16th project I worked on in the TripleTen Data Science program. A telecom company needed a system of identifying customers that were churn risks. The results of this project could help the company improve customer retention and outcomes.

## Project Goals

The goal of the project was to explore the data in order to then produce a model to effectively identify customers likely to discontinue their service and then have the opportunity to offer them incentives to stay. This involved building a model to predict customer churn.


### The Data

- **Features**:
  - `customerID`: Unique identifier for each customer.
  - `BeginDate`: Start date of the customer’s service.
  - `EndDate`: End date of the customer’s service (if applicable).
  - `Type`: Contract type (e.g., month-to-month, two-year).
  - `PaperlessBilling`: Indicates paperless billing usage.
  - `PaymentMethod`: Method of payment (e.g., electronic check, mailed check).
  - `MonthlyCharges`: Monthly service charges.
  - `TotalCharges`: Total charges incurred by the customer.
  - `gender`: Customer gender.

- **Binary Features**:
  - `SeniorCitizen`
  - `Partner`
  - `Dependents`
  - `OnlineSecurity`
  - `OnlineBackup`
  - `DeviceProtection`
  - `TechSupport`
  - `StreamingTV`
  - `StreamingMovies`
  - `MultipleLines`
  - 

### The Process

1. Loaded the data and checked that the data is free of issues — there is no missing data, extreme values, and so on.
2. Analyzed the data for class imbalances, needed information, useless information, and any opportunities for feature engineering.
3. Implemented one hot encoding and created new columns based on `EndDate`. If this `EndDate` column had values, it meant the customer had left the company, creating an opportunity for target prediction from this data. 
4. Researched seasonality of data more closely.
5. Trained several different models to find the most successful one. The primary metric being AUC-ROC and the additional one being accuracy. Machine learning models included Logistic Regression, RandomForestClassifier, GradientBoosting, and MLPClassifier.
6. Performed hyperparameter tuning and regularization of the best model after feature selection.

## Results

The final model was a Gradient Boosting model with fine-tuned hyperparameters. This model also needed some gradient boosting regularization during training, with some feature selection done on the data set in order to use the most relevant data in making predictions. The final quality scores of this model when tested against the test set are as follows: Test AUC-ROC: 0.886 and Test Accuracy: 0.841.


## Conclusion

The project provided strategic insights for the marketing team at the fictional telecom company. The insights gained from this project have the potential to guide future marketing strategies and optimize customer retention. The high AUC-ROC score of .886 suggests that this model is ready to be implemented, or at least built off of. By sending customers with high churn risk discounts or special deals, this model could reduce churn by a significant degree. Please refer to the Jupyter Notebook for a detailed description of the results. Additionally, the CSV files are also included. 
