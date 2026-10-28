# Spotify Track Popularity Prediction

## Project Overview

This project explores whether a song's popularity on Spotify can be predicted using its audio characteristics. Using R and the tidymodels ecosystem, I developed and evaluated a machine learning model to investigate the relationship between a track's audio features and its popularity score.

The project combines exploratory data analysis, data preprocessing, ensemble modelling, model evaluation, and feature importance analysis. Beyond building a predictive model, the goal was to understand how informative audio characteristics are when predicting track popularity.

## Objectives

Explore the dataset and identify patterns in Spotify track popularity and audio characteristics.

Clean and preprocess the data, including handling missing values.

Develop a machine learning model to predict track popularity.

Tune and evaluate the model using cross-validation and a held-out test dataset.

Examine feature importance to identify which audio characteristics contribute most to the model's predictions.

## Tools and Technologies

R: Main programming language

tidyverse: Data manipulation, cleaning, and exploratory data analysis

tidymodels: Model development, preprocessing, hyperparameter tuning, and evaluation

## Methodology

1. Exploratory Data Analysis

I began by exploring the dataset to understand its structure, examine the distribution of track popularity, and investigate relationships between the available audio features and the target variable.

I also examined correlations between variables to better understand the data and inform the modelling process.

2. Data Cleaning and Preprocessing

I prepared the dataset for modelling by cleaning the data and handling missing values through imputation (mice).

3. Model Development

I developed an ensemble learning model (stacking model) to predict Spotify track popularity from its audio characteristics.

The modelling workflow included:

Feature preprocessing

Hyperparameter tuning to identify suitable model configurations

Cross-validation to assess model performance across different data splits

This approach helped me evaluate different modelling configurations and select a final model based on its predictive performance.

4. Model Evaluation

I evaluated the final model on a held-out test dataset using the coefficient of determination ((R^2)).

The model achieved an R² of 0.213 on the test dataset, indicating that it explained approximately 21.3% of the variation in track popularity scores.

This result suggests that the audio features used in the model provided some predictive information, but were not sufficient to explain most of the variation in popularity. Other factors not captured by these features may also be relevant.

5. Feature Importance Analysis

I examined feature importance to understand which audio characteristics were most informative for the model's predictions.

This analysis provided additional insight into the relationship between the available audio data and track popularity. 

## Results and Key Takeaways

Developed an end-to-end machine learning workflow in R, from data exploration and preprocessing to model evaluation.

Applied ensemble learning, cross-validation, and hyperparameter tuning.

Achieved an R² of 0.213 on the held-out test dataset.

Investigated feature importance to better understand which audio characteristics were most useful for prediction.

The results illustrate the limitations of predicting popularity from audio characteristics alone and highlight the importance of evaluating models on unseen data.

## Conclusion

This project gave me practical experience in building and evaluating a machine learning model using R and tidymodels. It also helped me explore the challenges of predicting a complex outcome such as music popularity using a limited set of input features.

The project demonstrates my approach to data analysis and predictive modelling, including data preparation, model selection, performance evaluation, and interpretation of model results.
