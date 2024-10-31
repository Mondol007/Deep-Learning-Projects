# Deep-Learning-Projects

## Time Series Forecasting using LSTM

### Climate Data Analysis with LSTM

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


### Microsoft Stock Forecasting with LSTM

- Loaded and filtered Microsoft stock data for date and close prices.
- Converted date strings to date-time objects and set the date as the index.
- Plotted closing prices over time.
- Created a function to generate sliding windows of data for training, using a specified look-back window.
- Prepared the data into windowed sets for training, validation, and testing.
- Defined and compiled an LSTM model with dense layers for stock price prediction, using Mean Squared Error loss and Adam optimizer.
- Trained the model, monitoring validation error across 100 epochs.
- Visualized predictions against actual values for training, validation, and test sets.
- Used recursive forecasting to predict future values based on previous predictions and plotted the results alongside original data.



### Weather Prediction with LSTM

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



## Diffusion Models (Experimentation)

### Quick Diffusion

- Loaded the CIFAR-10 dataset and filtered it to retain only images of class 1 (airplanes).
- Normalized the training images to a range of [-1, 1].
- Created a time series for noise and clarity to use during training.
- Defined functions to convert images, display examples, add noise, and generate time steps.
- Developed a convolutional neural network model with residual blocks, max pooling, and upsampling layers.
- Compiled the model using Adam optimizer and mean absolute error loss function.
- Implemented a prediction function to generate images from random noise through multiple timesteps.
- Trained the model using a custom training loop, incorporating noise into the images.
- Adjusted the learning rate dynamically after each training round and visualized the model's predictions.


### Stable Diffusion

- Loaded the Stable Diffusion pipeline and related models (VAE, tokenizer, UNet, and scheduler) onto the GPU.
- Defined functions for generating image latent from text prompts, decoding latent to images, and creating videos from image sequences.
- Generated images from a series of prompts using the prompt-to-image function.
- Encoded generated images into latent for further manipulation.
- Perturbed latent to create variations of generated images.
- Implemented a new scheduler for image-to-image generation, adjusting latents based on a starting timestep.
- Produced and displayed images based on modified latent and new prompts.

