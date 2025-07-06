# demand-forecasting-for-inventory-optimization

Hybrid XGBoost + LSTM Demand Forecasting

This project implements a hybrid time-series model using XGBoost and LSTM (PyTorch) to forecast weekly product demand. The goal is to reduce stockouts by 25% and optimize inventory planning using machine learning and deep learning techniques.
📦 Project Structure

# This is formatted as code

🚀 Objectives

    Predict weekly demand for products using historical data
    Minimize stockouts by accurate forecasting
    Enable dynamic inventory optimization decisions

🧰 Tools & Technologies

    Python
    XGBoost
    PyTorch
    pandas, NumPy, Matplotlib
    scikit-learn for preprocessing

🧪 How It Works
1. Data Preprocessing

    Lag features, rolling averages, and date parts are engineered.
    Data is normalized and split into training and test sets.

2. XGBoost Model

    Learns non-linear feature relationships.
    Predictions from XGBoost are added as inputs to the LSTM.

3. LSTM Model

    Captures sequential dependencies in the demand data.
    Trained using PyTorch on sequences of [xgb_prediction, actual_demand].

4. Forecasting

    Final predictions are inverse-transformed and plotted.
    These forecasts can be used to set reorder points or optimize stock levels.

📊 Output

The model outputs:

    Weekly demand forecast plot (predicted vs actual)
    Metrics: MAPE, RMSE (extendable)
    Inventory optimization recommendations (e.g., reorder week flags)

💡 Example Use Cases

    Inventory planning for retail chains
    Seasonal product restocking
    Dynamic reorder point adjustment

⚙️ Installation

git clone https://github.com/arunbretlee/hybrid-demand-forecasting.git
cd hybrid-demand-forecasting
pip install -r requirements.txt

