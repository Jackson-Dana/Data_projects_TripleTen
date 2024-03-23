# TripleTen Sprint 13 Project - Predicting Taxi Orders

This is the 13th project I worked on in the TripleTen Data Science program. This project was highly independent and provided a comprehensive understanding of taxi order behavior for the Sweet Lift Taxi company.

## Sweet Lift Taxi Company
The goal of the project was to analyze historical data on taxi orders at airports to predict the amount of taxi orders for the next hour. The aim is to attract more drivers during peak hours.

## The Data
The number of orders is in the `num_orders` column. Time data was stored in the datetime
 column. 

## The Process
1. Downloaded the data and resampled it by one hour.
2. Analyzed the data, noting significant trends such as the increase in the number of orders daily from March to the end of August, the peak days being Monday and Friday, and evident peaks at around midnight, 10 am, and 4 pm.
3. Trained various machine learning models with different hyperparameters. The test sample was 10% of the initial dataset. A random forest model, a gradient boosting model, an autoregressive moving average model were attempted. An autoregressive integrated moving average model, specifically a SARIMA model, was trained additionally, with the assumption that such a model would be superior.
4. Tested the data using the test sample and provided a conclusion. The RMSE metric on the test set should not be significantly more than 48 for the final model.

## Results
The results were explained at each step. An introduction and conclusion were written that outlined the work done and made suggestions for Sweet Lift Taxi company to consider in the future. The Jupyter Notebook included provides a full description of the results. The RandomForest model produced the best model in terms of RMSE on the test set. 

## Conclusion
The project provided strategic insights for the Sweet Lift Taxi company. The insights gained from this project have the potential to guide future strategies and optimize driver allocation during peak hours. Using the best model produced may allow for the company to allocate drivers for projected peaks. 

Please refer to the Jupyter Notebook for a detailed description of the results. 
