# TripleTen Sprint 14 Project - Sentiment Analysis of Movie Reviews

This is the 14th project I worked on in the TripleTen Data Science program. The project was developed for the Film Junky Union, a community for classic movie enthusiasts. The goal of the project was to develop a system for filtering and categorizing movie reviews, specifically to train a model to automatically detect negative reviews.

## The Goal

The objective was to use a dataset of IMBD movie reviews with polarity labelling to build a model for classifying positive and negative reviews. The target was to reach an F1 score of at least 0.85.

## The Data

The data was stored in the `imdb_reviews.tsv` file. It was provided by Andrew L. Maas, Raymond E. Daly, Peter T. Pham, Dan Huang, Andrew Y. Ng, and Christopher Potts. (2011). Learning Word Vectors for Sentiment Analysis. The 49th Annual Meeting of the Association for Computational Linguistics (ACL 2011). This dataset was too large to post here on github. The selected fields included:

- `review`: the review text
- `pos`: the target, '0' for negative and '1' for positive
- `ds_part`: 'train'/'test' for the train/test part of dataset, correspondingly

## The Process

The project involved several steps:

1. Loading and preprocessing the data.
2. Conducting an Exploratory Data Analysis (EDA) and concluding on the class imbalance.
3. Preprocessing the text data for modeling.
4. Training at least three different models for the given train dataset.
5. Testing the models for the given test dataset.
6. Composing a few original reviews and classifying them with all the models.
7. Checking for differences between the testing results of models in the above two points and trying to explain them.
8. Presenting the findings.

## Results

The results were explained at each step. An introduction and conclusion were written that outlined the work done and made suggestions for the Film Junky Union to consider in the future. The best model, Logistic Regression, achieved an accuracy score of 0.88, ROC-AUC score of 0.95, and F1 score of 0.88 with testing data. Additionally, the models tested generalized well on the original reviews composed for this task. 

## Conclusion

This project provided a comprehensive understanding of sentiment analysis and its application in classifying movie reviews. The insights gained from this project can be used by the Film Junky Union to automatically filter and categorize movie reviews, enhancing the user experience on their platform. The project also demonstrated the effectiveness of various machine learning algorithms in text classification tasks, providing a foundation for future work in this area. For a more detailed explanation of the project, including the code, visualizations, and in-depth analysis, please refer to the accompanying Jupyter Notebook file.
