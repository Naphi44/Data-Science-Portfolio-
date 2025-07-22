# Time Series Forecasting Project

## Business Objective
Develop a robust time‑series forecasting model to accurately predict [e.g. weekly sales/demand] over the next horizon, enabling stakeholders to optimize inventory planning, reduce stockouts, and improve operational efficiency.

## Project Overview
This project explores classical (ARIMA) and modern (Prophet) forecasting techniques applied to a historical time series dataset. You’ll find:
- A Jupyter notebook (`Time_Series_Forecasting.ipynb`) showcasing data cleaning, model building, evaluation, and visualization.
- A standalone Python script (`time_series_forecasting.py`) that wraps the core pipeline into reusable functions.

## Repository Structure
.
├── README.md
├── Time\_Series\_Forecasting.ipynb    # Exploratory analysis & modeling walkthrough
├── time\_series\_forecasting.py       # Production‑ready forecasting module
└── data/dc.csv                         # CSV File 


## Installation
1. Clone the repo:
   git clone [https://github.com/Naphi44/Data-Science-Portfolio-.git]
   cd Data-Science-Portfolio-

2. Create & activate a virtual environment:

   python3 -m venv venv
   source venv/bin/activate    # macOS/Linux
   venv\Scripts\activate       # Windows
   

3. Install dependencies
   pip install pandas numpy matplotlib statsmodels prophet
## Usage

### Jupyter Notebook

1. Launch:
   jupyter notebook Time_Series_Forecasting.ipynb

2. Step through the cells to:

   * Load and visualize the data
   * Perform stationarity checks and differencing
   * Fit ARIMA and Prophet models
   * Compare forecasts against a test set

### Python Module

You can also run the script directly:

python time_series_forecasting.py \
  --data-path data/dc.csv \
  --model arima \
  --forecast-horizon 12

Use `--help` to explore all available options.

## Results & Visualization

* Forecast plots are saved in the `outputs/` folder.
* Metrics (MAE, RMSE) printed to console for quick comparison.
