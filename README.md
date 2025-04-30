# PassengerFlowPredictor

This project implements a time series forecasting model using a Long Short-Term Memory (LSTM) neural network. It uses the **Air Passengers dataset**, which contains monthly totals of international airline passengers from **1949 to 1960**.

## Dataset
- Dataset used: `AirPassengers.csv`
- Columns:
  - `Month`: Date in YYYY-MM format
  - `Passengers`: Total international airline passengers per month

##  Model
- Model type: LSTM (Long Short-Term Memory)
- Frameworks: TensorFlow, Keras
- Input: Past 12 months of passenger data
- Output: Predicts the 13th month's passenger count

## Steps
1. Load and preprocess the dataset
2. Normalize passenger counts using MinMaxScaler
3. Create time series sequences (12 input months → 1 output month)
4. Build and train an LSTM model
5. Predict and visualize results
6. (Optional) Forecast next 12 months
7. Save the model for future use

##  Results
- Plotted actual vs predicted passenger counts
- Model shows good ability to follow the trend

##  Files
- `AirPassengers.csv` – the dataset
- `MonthlyAirPassengerForecast.ipynb` – main notebook
- `lstm_airpassenger_model.h5` – saved LSTM model (optional)

##  Requirements
- Python 3
- pandas
- numpy
- matplotlib
- scikit-learn
- tensorflow / keras

##  How to Run
1. Open the notebook in Google Colab or Jupyter
2. Run each cell in sequence
3. View the plots and prediction results
