# Sprint 17 Project - Predicting Customer Churn for Interconnect Telecom

This is the 16th project I worked on in the TripleTen Data Science program. Interconnect, a telecom company, needed a system of identifying customers that were churn risks. The results of this project could help the company improve customer retention and outcomes by offering promotional codes and special plan options to users planning to leave.

## Project Goals

The primary goal of this project was to build a binary classification model that effectively identifies customers at high risk of churning. By accurately predicting which customers are likely to discontinue their service, Interconnect can proactively offer incentives and special plan options to retain these customers and improve overall customer retention.

## Interconnect's Services

Interconnect mainly provides two types of services:

1. Landline communication. The telephone can be connected to several lines simultaneously.
2. Internet. The network can be set up via a telephone line (DSL, digital subscriber line) or through a fiber optic cable.

Some other services the company provides include:

- Internet security: antivirus software (DeviceProtection) and a malicious website blocker (OnlineSecurity)
- A dedicated technical support line (TechSupport)
- Cloud file storage and data backup (OnlineBackup)
- TV streaming (StreamingTV) and a movie directory (StreamingMovies)

The clients can choose either a monthly payment or sign a 1- or 2-year contract. They can use various payment methods and receive an electronic invoice after a transaction.

## The Data

The data consists of files obtained from different sources:

1. `contract.csv` — Contract information
2. `personal.csv` — The client's personal data
3. `internet.csv` — Information about Internet services
4. `phone.csv` — Information about telephone services

Each file contains a unique code assigned to each client in the `customerID` column.

The contract information is valid as of February 1, 2020.

## The Process

1. Loaded the data and checked that the data is free of issues — there is no missing data, extreme values, and so on.
2. Merged the four CSV files on the `customerID` column.
3. Analyzed the data for class imbalances, needed information, useless information, and any opportunities for feature engineering.
4. Implemented one hot encoding and created new columns based on `EndDate`. If this `EndDate` column had values, it meant the customer had left the company, creating an opportunity for target prediction from this data.
5. Researched seasonality of data more closely.
6. Trained several different models to find the most successful one. The primary metric being AUC-ROC and the additional one being accuracy. Machine learning models included Logistic Regression, RandomForestClassifier, GradientBoosting, and MLPClassifier.
7. Performed hyperparameter tuning and regularization of the best model after feature selection.

## Results

The final model was a Gradient Boosting model with fine-tuned hyperparameters and regularization applied during training. Feature selection was also performed to ensure that the most relevant data was used in making predictions. The model achieved impressive performance metrics when evaluated on the test set, with an AUC-ROC score of 0.886 and an accuracy of 0.841.

It's worth noting that random states were not consistently set throughout the project, which may lead to slight variations in the quality scores each time the model is run. While this does not significantly impact the overall results, it is an area for improvement in future iterations of the project to ensure full reproducibility.

## Conclusion

The project provided strategic insights for the marketing team at Interconnect telecom company. The insights gained from this project have the potential to guide future marketing strategies and optimize customer retention. The high AUC-ROC score of 0.886 suggests that this model is ready to be explored further with the goal of being implemented. Please refer to the Jupyter Notebook for a detailed description of the results. Additionally, the CSV files are also included. The next step would be to work with the marketing team to design and test targeted retention campaigns based on the model's predictions.

