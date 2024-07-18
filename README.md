Analysis of time series data is an important and popular topic in data science. However, for various practical reasons, we often need to go beyong just simple analysis of time series data and want to predict the future values of the time series . There are many classical statistical and machine learning models to choose from for forecasting time series data. In this project I am using a classical statistical model - seasonal ARIMA - to forecast the future values of a time series dataset. I am using the Monthly Milk Production dataset. This dataset contains measurements of milk production in pounds per cow per month from January 1962 to December 1975. I download the dataset and I split it into two subsets, one for training a model and another for testing the model's predictions. I use Pandas library to read the files, check and clean the data from missing values. I use statsmodels functions to test the data for stationarity and transform the data to remove any non-stationarity. I visualize the time series and infer the model hyperparameters from autocorrelation functions. I use seasonal ARIMA model from statsmodels library. Seasonal ARIMA is a classical time series forecasting model that works well with time series data that contain seasonal variations. I build the model using the hyperparameters infered from the autocorrelation plots. I then train the model on the train subset. I assess the model's performance by using the model to make predictions for the future values of the time series and then comparing the predictions with the test dataset. I then provide summary of my findings.

References:
For this project I used the following sources:
Theoretical methods underlying statistical time series models are well described in "Forecasting: Methods and Applications" by S. Makridakis, S.C. Wheelwright, R.J. Hyndman, and in "Forecasting: Principles and Practice" by R. J. Hyndman and G. Athanasopoulos.
Practical aspects of how to implement time series models in Python can be found in "Time Series Analysis with Python Cookbook" by Tarek A. Atwan, and in "Modern Time Series Forecasting with Python" by Manu Joseph.
