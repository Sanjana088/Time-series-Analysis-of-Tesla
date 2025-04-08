## Tesla Stock Price Forecasting using Time Series Modeling

This project presents a complete time series analysis and forecasting pipeline applied to Tesla (TSLA) stock prices, using historical data from 2019 to 2023. The analysis involves data wrangling, visualization, statistical testing, and ARIMA-based forecasting to gain insights into stock movement patterns and predict future values.



## Project Objectives

- Clean and preprocess Tesla stock data
- Analyze trends, volatility, and returns
- Test stationarity and transform the series as required
- Determine optimal ARIMA model parameters using ACF, PACF, and grid search
- Forecast future stock prices and evaluate model performance

---

## Tools & Technologies

- **Python**: Core programming language
- **Pandas & NumPy**: Data manipulation
- **Matplotlib & Seaborn**: Visualization
- **Statsmodels**: Time series modeling (ARIMA, ADF test)
- **scikit-learn**: Model evaluation (MSE, MAE)

---

## Dataset

- Source: `TSLA.csv` (Tesla historical stock prices)
- Columns: `Date`, `Open`, `High`, `Low`, `Close`, `Adj Close`, `Volume`
- Time Range: May 1, 2019 – May 1, 2023

---

## Key Components

### 1. **Data Preprocessing**
- Converted `Date` column to datetime format
- Set `Date` as the index
- Filtered the dataset for a specific analysis range
- Handled missing values using **linear interpolation**

### 2. **Descriptive Statistics**
- Calculated mean, variance, max/min for both `Adj Close` and daily returns
- Assessed volatility and return distribution

### 3. **Stationarity Testing**
- Applied **Augmented Dickey-Fuller (ADF)** test
- Differenced the data to achieve stationarity

### 4. **Modeling with ARIMA**
- Conducted **ACF and PACF** analysis to determine p, d, q parameters
- Performed **grid search** over multiple ARIMA configurations
- Selected the best model based on **AIC**

### 5. **Forecasting & Evaluation**
- Forecasted stock prices on the test set
- Evaluated the model using **Mean Squared Error (MSE)**
- Visualized forecasts vs. actual values

---

##  Results

- Best-fit ARIMA model selected based on lowest AIC
- Achieved reasonable predictive performance with visual and statistical validation
- Demonstrated stock price volatility and cyclic patterns over a 4-year period



