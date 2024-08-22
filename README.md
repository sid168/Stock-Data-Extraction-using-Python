# Stock-Data-Extraction-using-Python
A Python-based project for extracting and analyzing stock data using the yfinance library, including historical price data and stock information.

This repository contains a Python-based project focused on extracting and analyzing stock data using the `yfinance` library. The project is designed for data scientists and analysts interested in financial data analysis, enabling them to retrieve historical stock prices, current stock information, and perform basic visualizations.


## Introduction
Understanding and analyzing stock data is crucial for financial analysts, investors, and data scientists. This project simplifies the process of retrieving and working with stock data by using Python's `yfinance` library, which allows for easy extraction of stock information and historical data directly from Yahoo Finance.

## Features
- Extract current stock information (e.g., market cap, P/E ratio).
- Retrieve historical stock price data.
- Generate visualizations of stock trends over time.
- Analyze data using Pandas and Matplotlib.

## Installation

To run this project locally, you'll need to install the required Python libraries. You can install them using the following commands:

```bash
pip install yfinance
pip install pandas
pip install matplotlib
```


## Examples

### Extracting Stock Information
```python
import yfinance as yf

# Define the stock ticker symbol
ticker = 'AAPL'

# Get stock data
stock = yf.Ticker(ticker)

# Print basic information
print(stock.info)
```

### Retrieving Historical Data
```python
# Get historical market data
historical_data = stock.history(period="1y")

# Plot the historical data
historical_data['Close'].plot(title=f"{ticker} Stock Price")
```

