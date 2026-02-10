# Air Passengers Time Series Analysis
## This project analyzes the classic "AirPassengers" time series dataset using ARIMA modeling techniques. The analysis focuses on time series decomposition, stationarity testing, and building predictive models for airline passenger forecasting.

###  Dataset
  - Dataset: AirPassengers.csv
  - Description: Monthly totals of international airline passengers (1949-1960)
  - Time Period: January 1949 - December 1960
  - Frequency: Monthly data
  - Units: Thousands of passengers

### Analysis Pipeline
#### 1. Data Preprocessing
  - Set 'Month' column as datetime index
  - Convert index to proper datetime format
  - Resample data to annual frequency for aggregation

#### 2. Exploratory Data Analysis
  - Rolling Statistics: 12-month moving average calculation
  - Visualization:
    - Original time series plot
    - Rolling mean overlay for trend analysis
    - Log-transformed series visualization
    - First-order differencing plots
   
#### 3. Stationarity Testing
  - Augmented Dickey-Fuller (ADF) Test:
    - Applied to original series
    - p-value analysis for stationarity determination
    - Results: Initial series is non-stationary (p > 0.05)

### Forecasting
  - Forecast Horizon: 400 periods (approximately 33 years)
  - Method: Model-based prediction using fitted ARIMA parameters
  - Output: Extended time series with predictions

