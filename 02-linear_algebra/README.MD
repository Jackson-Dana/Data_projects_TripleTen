# TripleTen Sprint 11 Project - Machine Learning and Linear Algebra

This is the 11th project I worked on in the TripleTen Data Science program. The Sure Tomorrow insurance company could benefit from the results of several tasks with the help of Machine Learning in order to improve revenue and outcomes.

## Project Goals

The goal of the project was to solve the following tasks:

1. Find customers who are similar to a given customer. This will help the company's agents with marketing.
2. Predict whether a new customer is likely to receive an insurance benefit. Can a prediction model do better than a dummy model?
3. Predict the number of insurance benefits a new customer is likely to receive using a linear regression model.
4. Protect clients' personal data without breaking the model from the previous task. It's necessary to develop a data transformation algorithm that would make it hard to recover personal information if the data fell into the wrong hands. This is called data masking, or data obfuscation. The data should be protected in such a way that the quality of machine learning models doesn't suffer. 

### The Data

The dataset includes the following features: insured person's gender, age, salary, and number of family members. The target is the number of insurance benefits received by an insured person over the last five years.

### The Process

1. Loaded the data and checked that the data is free of issues — there is no missing data, extreme values, and so on.
2. Worked on each task and answered the questions posed in the project template.
3. Drew conclusions based on my experience working on the project.

## Results

The results were explained at each step. An introduction and conclusion were written that outlined the work done and made suggestions for Sure Tomorrow to consider in the future. 

1. Found customers similar to a given customer and then trained a model to predict if a new customer will need benefits. The trained model does better than the dummy model.
2. Predicted the number of insurance benefits a customer is likely to receive using a linear regression model. It was successful, and then I showed that the R2 value is not impacted by scaling when using a linear regression model.
3. Protected the clients' data through obfuscation without impacting the quality of the data or the ability to train models on the data.

## Conclusion

The project provided strategic insights for the marketing team at Sure Tomorrow. The insights gained from this project have the potential to guide future marketing strategies and optimize revenue generation. The clients' data was also protected through obfuscation without impacting the quality of the data or the ability to train models on the data. Please refer to the Jupyter Notebook for a detailed description of the results.
