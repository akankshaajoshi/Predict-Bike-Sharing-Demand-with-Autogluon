## Predict Bike Sharing Demand Using AutoGluon
Bike sharing is a regression time-series problem which predicts the count of bike sharing depending on the previously forecasted trends. The model employs the following techniques:

1. Data gathering: Download command for the dataset using Kaggle API is - kaggle competitions download -c bike-sharing-demand
2. Data wrangling: Includes cleaning of dataframe, conversion of features to proper feature values - assigning categorical and datetime data type to respective columns.
3. Exploratory data analysis: Summary statistics and describe methods give an overview of the data distribution. Histogram of each individual feature gives an idea about the underlying data distribution.
4. Model selection: Using Autogluon Predictor, dataset is loaded and fitted into a number of different predictive models and statistics of model features is recorded with the achieved accuracy.
5. Hyperparameter tuning: Hyperparameter tuning using differnet set of parameters on the top ranking models in the leaderboard further enhances the performance of the highest performing models.

Multiple models are evaluated with the presets achieving best accuracy over a time limit of 600 seconds. Final prediction scores are evaluated and it is seen that the ##hyperparameter optimized model performs better than the other models. Thus, it's used to make prediction using WeightedEnsemble_L3. 

Scores achieved on the models are:
On the training set
![model_train_score](https://github.com/akankshaajoshi/Predict-Bike-Sharing-Demand-with-Autogluon/assets/91690660/f35fc805-f18d-4c72-9884-13a1d6ea79c0)

On the test set
![model_test_score](https://github.com/akankshaajoshi/Predict-Bike-Sharing-Demand-with-Autogluon/assets/91690660/cc3805e3-87d6-4b6b-9667-457df25a8a6c)
