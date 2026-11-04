# Assignment 4 – LSTM-Based Time-Series Forecasting

## Aim

To develop an LSTM-based model for time-series forecasting using a sales dataset.

## Objective

- Understand time-series forecasting.
- Load and explore sales data.
- Perform data preprocessing and normalization.
- Create sequences for LSTM input.
- Build an LSTM neural network using TensorFlow/Keras.
- Train the model and generate predictions.
- Evaluate the model using MAE and RMSE.
- Visualize actual and predicted sales.

## Dataset

The Monthly Shampoo Sales dataset was used.

### Dataset Details

- Total observations: 36
- Feature: Monthly sales
- Data type: Time-series data
- Training records: 28
- Testing records: 8

## Libraries Used

- TensorFlow
- Keras
- NumPy
- Pandas
- Matplotlib
- Scikit-learn

## Tasks Performed

### 1. Dataset Loading and Exploration

Loaded the Monthly Shampoo Sales dataset using Pandas and explored its statistical properties.

### 2. Data Visualization

Created a line graph to visualize monthly shampoo sales and identify trends and fluctuations.

### 3. Data Preprocessing

Extracted the sales values and normalized them using MinMaxScaler.

### 4. Sequence Creation

Created time-series sequences using the previous 3 months of sales data to predict the next month's sales.

### 5. Train-Test Splitting

Divided the sequences chronologically into training and testing datasets.

### 6. LSTM Model Development

Developed an LSTM model using TensorFlow/Keras with:

- Input shape: 3 time steps, 1 feature
- LSTM layer: 50 units
- Output layer: 1 neuron
- Optimizer: Adam
- Loss function: Mean Squared Error

### 7. Model Training

Trained the LSTM model for 100 epochs using a batch size of 4.

### 8. Prediction

Generated sales predictions using the trained LSTM model and compared them with actual sales values.

### 9. Model Evaluation

The model was evaluated using:

- Mean Absolute Error (MAE): 71.84
- Root Mean Squared Error (RMSE): 89.57

### 10. Visualization

Created graphs for:

- Monthly Shampoo Sales
- Actual vs Predicted Shampoo Sales
- LSTM Model Training Loss

## Analysis

The dataset showed an overall increasing trend in shampoo sales with fluctuations over time.

The training loss decreased significantly during the initial epochs and gradually stabilized as training progressed.

The actual and predicted sales graph was used to compare the forecasting performance of the LSTM model.

The model achieved an MAE of 71.84 and an RMSE of 89.57 on the test dataset.

## Conclusion

An LSTM-based time-series forecasting model was successfully developed using the Monthly Shampoo Sales dataset.

The assignment demonstrated data preprocessing, sequence creation, LSTM model development, training, prediction, and performance evaluation.

The practical implementation provided an understanding of how LSTM networks can be used for time-series forecasting.
