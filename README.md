# Stock-market-price-LSTM
This code imports necessary libraries, preprocesses stock data, builds and trains an LSTM model for stock price prediction, and visualizes training and test results, including future value prediction.
# Explaination 
This code performs the following tasks:

1. **Importing Libraries**: It imports necessary Python libraries for data manipulation, visualization, and machine learning using Keras.

2. **Data Loading and Inspection**: It loads Apple stock data from a CSV file, reverses the order of rows, and inspects the data by displaying its first few rows, data types, summary statistics, and shape. It also checks for missing values and fills them with zeros.

3. **Data Visualization**: It creates various data visualizations such as histograms, scatter plots, box plots, and time series plots to analyze the data's distribution, relationships, and trends.

4. **Data Exploration**: It calculates skewness and kurtosis to assess data distribution asymmetry and tail behavior, and it analyzes categorical variables by counting unique values.

5. **Correlation Analysis**: It calculates and visualizes the correlation matrix of numeric columns, allowing for insights into variable relationships.

6. **Feature Engineering**: It creates lag features for daily returns, including 1-day and 2-day returns, and calculates a 20-day simple moving average.

7. **Time Series Data Preparation**: It scales the data using Min-Max scaling, splits it into training and test datasets, and prepares the data as time series sequences for LSTM modeling.

8. **LSTM Model Definition**: It defines an LSTM neural network model using Keras with two LSTM layers and an output layer with linear activation.

9. **Model Compilation and Training**: It compiles the model with mean squared error loss and the Adagrad optimizer, then trains the model on the training data for a specified number of epochs.

10. **Prediction and Evaluation**: It makes predictions on both the training and test datasets and calculates root mean squared error (RMSE) to evaluate the model's performance.

11. **Data Plotting**: It creates plots to visualize the original OHLC values, training predictions, and test predictions.

12. **Future Value Prediction**: It predicts future values by taking the last predicted value, scaling it, and using it as input to the trained model.

    The code combines data exploration, feature engineering, LSTM modeling, and visualization to analyze and predict Apple stock prices.
