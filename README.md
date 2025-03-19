# Alpha-Vantage-API
## Stock Market Data Analysis using Alpha Vantage API
### Overview

This Jupyter Notebook fetches stock market data using the Alpha Vantage API and processes it with pandas. Additionally, it includes web scraping functionality using BeautifulSoup.

### Features

Retrieves monthly and weekly stock data for Microsoft (MSFT).

Uses Alpha Vantage API for real-time stock data.

Implements web scraping with BeautifulSoup.

Processes and analyzes stock data with pandas.

### Requirements

To run this notebook, install the necessary dependencies:

```bash
pip install alpha_vantage requests beautifulsoup4 pandas
```


### Setup

Get an API Key from Alpha Vantage.

Save the key in a text file (API_key.txt).

Run the notebook to fetch and analyze stock data.

### Usage

Run each cell sequentially.

Modify the stock symbol to fetch data for different companies (MSFT: Microsoft).

Use pandas to further analyze or visualize the data.

Example Code Snippet

# Open file with API key
```bash
with open('API_key.txt') as file:
    API_key = file.read().strip()
```

# Import required libraries
```bash
from alpha_vantage.timeseries import TimeSeries
import pandas as pd
```

# Fetch stock data 
```bash
ts = TimeSeries(key=API_key)
data, meta_data = ts.get_monthly('MSFT')
```

