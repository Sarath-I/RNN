# Building a Simple RNN Model for Weather Temperature Prediction
🌦️ Weather Temperature Forecasting using SimpleRNN
📌 Project Overview

This project implements a Recurrent Neural Network (RNN) using TensorFlow/Keras to forecast the next day's temperature based on historical weather data.

The model leverages time-series patterns from past weather conditions such as temperature, humidity, and wind speed to predict future temperature trends. This project demonstrates practical implementation of sequence modeling using SimpleRNN for regression tasks.

🎯 Objective

The primary goal of this project is to:

Design and implement a SimpleRNN-based time series forecasting model

Predict the next day's temperature

Evaluate model performance using standard regression metrics

Forecast future temperature trends (next 7 days)

📊 Dataset

The model uses a Daily Weather Dataset containing:

📅 Date

🌡️ Temperature (Target Variable)

💧 Humidity

🌬️ Wind Speed

🌡️ Pressure (Optional Feature)

🛠️ Project Workflow
🔹 Part A: Data Understanding & Preprocessing

Loaded and explored the dataset

Visualized temperature trends over time

Checked and handled missing values

Applied MinMaxScaler for normalization

Created time sequences using past 7–14 days of weather data

Split data into Training, Validation, and Test sets

🔹 Part B: Model Development

The model architecture includes:

Input Layer (Sequence Length × Features)

SimpleRNN Layer (32–64 units)

Dropout Layer (to prevent overfitting)

Dense Output Layer (1 unit – Linear activation)

Model Compilation:

Loss Function: Mean Squared Error (MSE)

Optimizer: Adam

Metrics: Mean Absolute Error (MAE)

Training Configuration:

Batch Size: 32

Epochs: 50–100

Validation monitoring for performance tracking

Training and validation loss curves were plotted to analyze learning behavior.

🔹 Part C: Model Evaluation & Forecasting

Model performance was evaluated on the test dataset using:

📉 RMSE (Root Mean Squared Error)

📊 MAE (Mean Absolute Error)

📈 R² Score

Additional visualizations include:

Predicted vs Actual Temperature comparison

7-Day Temperature Forecast

Historical vs Forecasted trend visualization

📈 Results

The SimpleRNN model successfully captured temporal patterns in weather data and generated reliable short-term forecasts. Performance metrics indicate strong predictive capability for daily temperature forecasting.

🚀 Technologies Used

Python

TensorFlow / Keras

NumPy

Pandas

Matplotlib

Scikit-learn
