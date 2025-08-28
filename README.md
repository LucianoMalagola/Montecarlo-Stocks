# Montecarlo Stocks Price Simulator
A Python tool for simulating future stock prices or currency exchange values using Monte Carlo methods, with data from Yahoo Finance.

## DISCLAIMER

**I am NOT a financial advisor. This project is for educational purposes only and should NOT be considered financial advice. Always do your own research before making investment decisions.**

## Functions
- This tool download historical stock data from Yahoo Finance based on user input for a specific company (e.g. TSLA) or currency exchange (e.g. USDEUR=X), even S&P 500 data (^GSPC).
- Analysis is evaluated over a selected range (in years or months).
- The Monte Carlo simulation is used to predict future stock prices based on historical data.
- The simulation results are visualized over a horizon of 7 days.

# Highlights
- The tool calculates and displays key statistics:
  - Historic max, min, mean, standard deviation, last price of stock
  - Daily mean return (μ)
  - Daily standard deviation (σ)
  - Estimated beta (β)
    - Calculated over the selected period, relative to the S&P 500.

- Displays visualization of:
  - Historical price chart
  - Monte Carlo simulation fan chart
  - Mean and median simulated price lines
  - Prints 95% confidence intervals, mean, and median for each simulated day

## Python Libraries Used
- pandas for data manipulation.
- numpy for numerical calculations.
- matplotlib for plotting graphs.
- yfinance to fetch stock data.
- relativedelta to manipulate date ranges and consider leap years and holidays (for accurate analysis).

## Goals and Improvements
- Add more user controls for simulation parameters (e.g., custom forecast horizon, number of simulations)
- Allow for additional statistical outputs and risk metrics
- Improve error handling and support for more ticker formats
- Enhance visualizations with interactive charts (e.g., Plotly)

And finally...

- **Get to release a web-based tool using [Streamlit](https://streamlit.io/)** for an interactive, user-friendly experience—making the Monte Carlo simulator accessible to anyone without coding skills.
