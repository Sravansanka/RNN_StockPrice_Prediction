
# Stock Price Prediction using RNN and LSTM Models

## Overview
This project focuses on predicting stock closing prices for major technology companies: Amazon (AMZN), Google (GOOGL), IBM, and Microsoft (MSFT) using Recurrent Neural Networks (RNN) and Long Short-Term Memory Networks (LSTM). Historical daily stock data from 2006 to 2018 was used to train, validate, and test the models.

## Problem Statement
The objective is to develop models capable of predicting stock prices for one or more companies simultaneously, based on previous historical data. Two modeling approaches were explored:
- Simple RNN models
- Advanced LSTM models

Both single-output (one company) and multi-output (multiple companies) prediction setups were implemented and evaluated.

## Project Structure
- **Data Loading and Preparation:**
  - Aggregation of datasets
  - Scaling, window creation, and sequence generation
- **Model Development:**
  - Simple RNN Model
  - Advanced RNN Model (LSTM architecture)
- **Hyperparameter Tuning:**
  - Number of RNN units, batch size, learning rate
- **Evaluation Metrics:**
  - Mean Squared Error (MSE)
  - Mean Absolute Error (MAE)
  - R-squared Score (R²)
- **Visualization:**
  - Loss curves
  - Actual vs Predicted stock prices

## Technologies Used
- Python 3
- TensorFlow/Keras
- Pandas
- NumPy
- Scikit-learn
- Matplotlib

## Key Outcomes
- LSTM models significantly outperformed Simple RNNs in capturing stock price movements.
- Multi-output LSTM models were able to predict multiple stocks simultaneously with high accuracy for AMZN, GOOGL, and MSFT.
- IBM predictions were comparatively less accurate, suggesting the need for deeper modeling or additional features.
- Proper scaling, appropriate window sizes, and early stopping were critical to achieving stable model performance.

## Final Evaluation Metrics (Multi-Output LSTM)

| Stock        | Mean Squared Error (MSE) | Mean Absolute Error (MAE) | R² Score |
|--------------|--------------------------|----------------------------|------------|
| CloseAMZN    | 3145.17                   | 37.72                      | 0.9023     |
| CloseGOOGL   | 786.32                    | 20.30                      | 0.9384     |
| CloseIBM     | 105.74                    | 8.80                       | 0.3210     |
| CloseMSFT    | 19.46                     | 3.12                       | 0.8299     |

## How to Run
1. Install dependencies listed in the `requirements.txt` (if applicable).
2. Open the Jupyter notebook provided.
3. Run the cells sequentially to load data, build models, tune hyperparameters, and evaluate results.
4. Review the graphs and metrics produced for insights.

## Authors
**Sravana Kumar Sanka**  
**Srikrishna Jana**
