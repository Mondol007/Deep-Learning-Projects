# Deep-Learning-Projects

## Time Series Forecasting using LSTM

### Climate_Data_Analysis_with_LSTM

- Loaded the Climate dataset from TensorFlow and converted the date column to the index for time series analysis.
- Visualized temperature data over time.
- Created a sliding window function to generate training samples and labels for temperature forecasting.
- Split data into training, validation, and test sets.
- Built and summarized an LSTM model with two dense layers for regression.
- Compiled the model with Mean Squared Error loss and Root Mean Squared Error as the metric, using Adam optimizer.
- Trained the model with checkpoints to save the best version.
- Evaluated the model on training, validation, and test sets, comparing predictions against actuals.
- Visualized predictions vs. actuals for training, validation, and test results.
- Calculated Mean Squared Error for test predictions using a helper function.


### Microsoft_Stock_Forecasting_with_LSTM

- Loaded and filtered Microsoft stock data for date and close prices.
- Converted date strings to date-time objects and set the date as the index.
- Plotted closing prices over time.
- Created a function to generate sliding windows of data for training, using a specified look-back window.
- Prepared the data into windowed sets for training, validation, and testing.
- Defined and compiled an LSTM model with dense layers for stock price prediction, using Mean Squared Error loss and Adam optimizer.
- Trained the model, monitoring validation error across 100 epochs.
- Visualized predictions against actual values for training, validation, and test sets.
- Used recursive forecasting to predict future values based on previous predictions and plotted the results alongside original data.



### Weather_Prediction_with_LSTM

- Loaded a weather dataset and performed data cleaning by removing columns with insufficient non-null values.
- Converted the date column to a date-time format and sorted feature columns by non-null counts.
- Visualized the presence of features over time with scatter plots.
- Selected relevant features and attributes, then dropped rows with incomplete data.
- Defined columns for imputation methods and set up a cross-validation framework to compare RMSE for various imputation techniques.
- Calculated the correlation matrix of imputed features and visualized it with a heatmap.
- Implemented a function to prepare multivariate time series data for model training.
- Split data into training, validation, and test sets, standardizing it based on the training split.
- Built an LSTM model, trained it, and plotted the training/validation accuracy and loss.
- Predicted and visualized temperature forecasts from the model.

