# stock-price-prediction
This project implements a CNN-LSTM model to predict stock prices for the next day, and the next 5 days using historical stock data


# Stock Prediction Using CNN-LSTM

This project implements a Convolutional Neural Network (CNN) and a CNN-LSTM model to predict stock prices using historical stock data from Yahoo Finance. The goal is to predict stock prices for the next 5 days based on past stock price data.

Here’s a sample `README.md` file for your Stock Prediction Project. This README will provide a clear introduction, setup instructions, and usage guidelines for users and collaborators.

### Sample `README.md` File

```markdown
# Stock Prediction Using CNN-LSTM

This project implements a Convolutional Neural Network (CNN) and a CNN-LSTM model to predict stock prices using historical stock data from Yahoo Finance. The goal is to predict stock prices for the next 5 days based on past stock price data.

## Table of Contents
- [Project Overview](#project-overview)
- [Getting Started](#getting-started)
- [Model Architecture](#model-architecture)
- [Installation](#installation)
- [Usage](#usage)
- [Results](#results)
- [Contributing](#contributing)
- [License](#license)

## Project Overview

This project uses stock market data from Yahoo Finance to train deep learning models (CNN and CNN-LSTM) for stock price prediction. The models take the past 60 days of stock prices as input and forecast the next 5 days.

### Objectives:
- Fetch stock market data from Yahoo Finance using the `yfinance` library.
- Build and train CNN and CNN-LSTM models using historical data.
- Forecast stock prices for the next 5 days.
- Evaluate the models based on Mean Squared Error (MSE), Mean Absolute Error (MAE), and R² score.

## Model Architecture

### CNN (Convolutional Neural Network)
- Convolutional and MaxPooling layers to extract features from stock price sequences.
- Dense layers to predict the next 5 days' closing prices.

### CNN-LSTM (Convolutional Long Short-Term Memory)
- TimeDistributed CNN layers followed by LSTM layers to capture both spatial and temporal dependencies in the data.

## Getting Started

Follow the instructions below to set up and run the project on your local machine.

### Prerequisites

Ensure you have the following libraries installed:
- `numpy`
- `pandas`
- `yfinance`
- `matplotlib`
- `scikit-learn`
- `tensorflow`

You can install these dependencies by running the following command:
```bash
pip install -r requirements.txt
```

Alternatively, you can install the dependencies individually using `pip`:
```bash
pip install numpy pandas yfinance matplotlib scikit-learn tensorflow
```

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/YourUsername/YourRepositoryName.git
   ```
   
2. Navigate into the project directory:
   ```bash
   cd YourRepositoryName
   ```

3. Install the necessary dependencies (if not already done):
   ```bash
   pip install -r requirements.txt
   ```

## Usage

Once the dependencies are installed, you can run the Jupyter Notebook (`Stock_Prediction_Project.ipynb`) to train the models and make predictions.

1. Launch Jupyter Notebook:
   ```bash
   jupyter notebook
   ```

2. Open the `Stock_Prediction_Project.ipynb` file in the browser.

3. Modify the ticker symbol or date ranges as needed, and run the cells to train the models and forecast stock prices.

### Key Steps in the Notebook:
- **Data Collection**: Download stock data using the `yfinance` library.
- **Data Preprocessing**: Normalize and structure the data for time-series prediction.
- **Model Training**: Train CNN and CNN-LSTM models using TensorFlow/Keras.
- **Evaluation**: Evaluate the models using MSE, MAE, and R² score.
- **Visualization**: Plot the predicted vs. actual stock prices.

## Results

The models provide forecasts for the next 5 days of stock prices. Below are example evaluation metrics for the CNN and CNN-LSTM models:

- **Mean Squared Error (MSE)**: Measures the average squared difference between actual and predicted prices.
- **Mean Absolute Error (MAE)**: Measures the average magnitude of the prediction errors.
- **R² Score**: Represents how well the model predictions explain the variability in the actual stock prices.

### Example Visualizations:
The notebook generates visualizations that compare the predicted and actual stock prices for each day in the 5-day forecast.

![Sample Plot](https://github.com/YourUsername/YourRepositoryName/sample-plot.png)

## Contributing

Contributions are welcome! If you would like to contribute to this project, please fork the repository and create a pull request with your changes.





