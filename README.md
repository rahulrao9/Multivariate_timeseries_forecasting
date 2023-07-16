# Multivariate Time-Series Forecasting using LSTM for Small Datasets
This repository demonstrates the application of Long Short-Term Memory (LSTM) models for multivariate time-series forecasting, specifically designed for small datasets. The LSTM model is a powerful tool for capturing temporal dependencies in data, making it ideal for predicting future values in multivariate time-series data.

### Dataset
Before diving into the forecasting process, it is crucial to properly preprocess the dataset. This includes handling missing values, scaling variables, and splitting the data into training and testing sets. It's important to note that small datasets have limited information, higher noise levels, and less representative patterns compared to larger datasets. Hence, handling them with care is essential.

### Model Architecture
The core of this project lies in designing an effective LSTM architecture for multivariate time-series forecasting. The steps involved are as follows:

**Import the necessary libraries**: TensorFlow or Keras for building the LSTM model, Pandas for data manipulation, and Matplotlib for data visualization.

**Load and preprocess the dataset**: Load the dataset into a Pandas DataFrame and perform necessary preprocessing steps, such as handling missing values, scaling variables, and splitting it into train and test sets.

**Define the LSTM architecture**: Specify the number of LSTM layers, hidden units, and other hyperparameters. Design the input shape based on the number of features and time steps.

**Compile and train the model**: Compile the model with an appropriate loss function and optimizer. Train the model using the training set and validate it on the testing set. Monitor the training progress and adjust hyperparameters if needed.

**Make predictions**: Utilize the trained LSTM model to forecast future values. Due to the limitation of forecasting only one value for a column at a time, recursively call the forecasting function and append the predicted values to the original dataset. It is advisable to limit the forecast to a relatively small number of values in the future to maintain reasonable accuracy.

**Visualize the results**: Plot the predicted values against the actual values to visually assess the model's performance. Ensure the graph is easy to understand and contains relevant labels, titles, and legends.

### Repository Structure
Contains the dataset files used for training and testing the LSTM model.
Jupyter notebooks demonstrating the step-by-step process of data preprocessing, model building, training, and forecasting.

### Usage

Navigate to the notebooks directory and run the Jupyter notebooks to follow the step-by-step process.
Customize the code to fit your own dataset by editing the relevant sections.
Experiment with different hyperparameters, preprocessing techniques, and model architectures to achieve optimal results.
Document your findings, insights, and observations in the notebooks and share them with the community.
Feel free to explore the code, experiment with different datasets, and adapt it to your specific needs. I hope this repository serves as a helpful resource for understanding and implementing multivariate time-series forecasting using LSTM for small datasets.

***If you find this repository useful, kindly consider giving it a star ⭐️ and acknowledging the original author.***

> Note: It's important to acknowledge that the accuracy and reliability of the forecasting model may be limited by the size and characteristics of the dataset. Carefully evaluate the model's performance and make necessary adjustments based on your specific requirements.
