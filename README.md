# Deep-Learning-Projects

## Time Series Forecasting using LSTM

### Climate_Data_Analysis_with_LSTM

- Loaded Climate dataset from TensorFlow and converted the date column to the index for time series analysis.
- Visualized temperature data over time.
- Created a sliding window function to generate training samples and labels for temperature forecasting.
- Split data into training, validation, and test sets.
- Built and summarized an LSTM model with two dense layers for regression.
- Compiled the model with Mean Squared Error loss and Root Mean Squared Error as the metric, using Adam optimizer.
- Trained the model with checkpoints to save the best version.
- Evaluated the model on training, validation, and test sets, comparing predictions against actuals.
- Visualized predictions vs. actuals for training, validation, and test results.
- Calculated Mean Squared Error for test predictions using a helper function.
