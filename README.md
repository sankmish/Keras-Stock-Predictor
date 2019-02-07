# Keras-Stock-Predictor
A repository to store progress on Machine Learning project on DOW Jones stock data compiled by Sanket Mishra, Meenakshi Kavaseri, Eric Hagee, Brian Klovert, and Shagufta Zareen

![LSTM image](https://github.com/sankmish/Keras-Stock-Predictor/blob/master/images/LSTM-30:5.png)

# Project Description
This project uses data obtained from [Kaggle](https://www.kaggle.com/timoboz/stock-data-dow-jones) about the stocks in the Dow Jones industrial
average to investigate stock predictions by various machine learning algorithms.  As a beginning, we tested and developed models on one stock
chosen at random, Wal-Mart (stock code: WMT).

Methods investigated included:
 - Moving Average
 - ARIMA
 - K-Nearest Neighbors
 - SVM
 - Linear and Logistic Regression
 - Deep Neural Network
 - Deep Long-Short Term Memory (LSTM) Network
 
In the end, the LSTM model seems to show the most promise, but can only give semi-decent predictions for short days in the future, with variation between individual models.
As a standard, we used 30 days data to predict 5 days in the future for all 30 stocks in the Dow Jones Industrial Average.
We found similar results for all 30 stocks.

Future work would likely require further extensive tuning of the LSTM model and new data sources such as more years of stocks and different types of stocks as a first step.
As well, while an LSTM model has properties that recommend it for a time-series model, it may not be the best method.

# File Structure
The most important folders and files are as follows:
 - The Resources folder contains the 30 csv files obtained from Kaggle (with data up to on or about Jan. 25, 2019).
 - The LSTM folder contains the development of the LSTM model as follows:
  * The development of the model is contained in the Jupyter notebook file LSTMNotebook.ipynb
  * The use of the model for all 30 stocks is contained in the file LSTM_Stock_Analysis.ipynb
  * Various models are saved in .h5 format.
 - The Jupyter notebook file filter_data_and_models.ipynb contains a summarization of all models used.
 - Various models developed are saved in .h5 format in the main folder.
 - A summary of the project is in Keras Stock Predictor.pptx.
 - The images folder contains images for use in this README file.
