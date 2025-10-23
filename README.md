# Montecarlo Stocks Price Simulator
A Python tool for simulating future stock prices or currency exchange values using Monte Carlo methods, with data from Yahoo Finance.

<p align="center">
  <img src="https://raw.githubusercontent.com/LucianoMalagola/Montecarlo-Stocks/refs/heads/main/Montecarlo%20pictures/5M.png" width="59%" alt="5M">
</p>

##### DISCLAIMER: **I am NOT a financial advisor. This project is for educational purposes only and should NOT be considered financial advice. Always do your own research before making investment decisions.**

## Functions
- This tool downloads historical stock price data from Yahoo Finance based on user input for a specific company (e.g. AAPL for Apple) or currency exchange (e.g. USDEUR=X for USD/EUR). -> **_Up to 20 full years / 240 full months._**
- Analysis is evaluated over a selected range (in years or months).
- The Monte Carlo simulation is used to predict future stock prices based on historical data.
- The simulation results are visualized over a horizon of 7 days.

<p align="center">
  <img src="https://raw.githubusercontent.com/LucianoMalagola/Montecarlo-Stocks/refs/heads/main/Montecarlo%20pictures/1M.png" width="60%" alt="1M">
</p>

<p align="center">
  <img src="https://raw.githubusercontent.com/LucianoMalagola/Montecarlo-Stocks/refs/heads/main/Montecarlo%20pictures/3M.png" width="39%" alt="3M">
  <img src="https://raw.githubusercontent.com/LucianoMalagola/Montecarlo-Stocks/refs/heads/main/Montecarlo%20pictures/7M.png" width="59.5%" alt="7M">
</p>

# Highlights
- The tool calculates and displays key statistics:
  - Historic max, min, mean, standard deviation, last price of stock.
  - Daily mean return (μ).
  - Daily standard deviation (σ).
  - Estimated beta (β).
    - Calculated over the selected period using linear regression, relative to the market (S&P 500).

<p align="center">
  <img src="https://raw.githubusercontent.com/LucianoMalagola/Montecarlo-Stocks/refs/heads/main/Montecarlo%20pictures/4M.png" width="45%" alt="4M">
</p>

- Displays visualization of:
  - Historical price chart.
  - Monte Carlo simulation fan chart.
  - Mean and median simulated price lines.
  - Prints 95% confidence intervals, mean, and median for each simulated day.

<p align="center">
  <img src="https://raw.githubusercontent.com/LucianoMalagola/Montecarlo-Stocks/refs/heads/main/Montecarlo%20pictures/6M.png" alt="6M">
</p>

## Python Libraries Used
- pandas for data manipulation.
- numpy for numerical calculations.
- matplotlib for plotting graphs.
- yfinance to fetch stock data.
- relativedelta to manipulate date ranges for more flexible time calculations (for accurate analysis).
- sklearn.linear_model to calculate the stock's beta (β) relative to the market using Linear Regression. 

## Goals and Improvements
- Add more user controls for simulation parameters (e.g., custom forecast horizon, number of simulations).
- Allow for additional statistical outputs and risk metrics.
- Enhance visualizations with interactive charts (e.g. Plotly).
