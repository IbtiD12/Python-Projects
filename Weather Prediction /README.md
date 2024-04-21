For this project, I used the London weather dataset from 1979 to 2021. The goal is to automatically process and test different models using sklearn and MLflow.

The result of this project is an MLflow experiment with three different regression models (linear regression, decision tree regressor, and random forest regressor) and their results.

We will log the RMSE scores for each model as a metric called rmse_{{model}}, where {{model}} is replaced with lr, tr, and fr for linear regression, decision tree regressor, and random forest regressor respectively.

Perform exploratory data analysis, preprocessing, training, prediction, and evaluation of machine learning models to predict "mean_temp" from the london_weather.csv, logging models, metrics, and parameters to a MLflow experiment. perform exploratory data analysis to identify suitable features for predicting modeling. Store selected features in feature_selection and the target variable as target_var.

Define a function called preprocess_df(), which takes three arguments: df- the DataFrame for preprocessing; feature_selection - the features to subset the DataFrame on; and target_var - the target variable for the predictive model. Define a function predict_and_evaluate(), which takes three arguments: model - a pre-trained ML model; x_test and y_test - test set for independent variables and labels respectively. The function should predict values from the test set for the particular model, and calculate and return the root mean squared error (RSME).

Complete the for loop for varying depths, where I train the models, evaluate their performance using the predict_and_evaluate() function, and log their performance using the current depth.
