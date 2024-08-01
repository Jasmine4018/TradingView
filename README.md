# TradingView Stock Data Fetcher

This Python script fetches stock data from the TradingView Market Movers page and saves it to an Excel file. It continuously updates the data at regular intervals during specified hours.

## Features

- Fetches stock data from TradingView's active market movers page.
- Parses the data and appends it to an Excel file.
- Runs at regular intervals between specified start and end times.

## Requirements

- Python 3.x
- `requests` library
- `beautifulsoup4` library
- `pandas` library
- `openpyxl` library
- `pytz` library

## Installation

1. **Clone the repository or download the script.**

2. **Install the required libraries:**
   ```bash
   pip install requests beautifulsoup4 pandas openpyxl pytz

Configuration
URL: The URL to fetch stock data from TradingView's Market Movers page.
FILE_PATH: The path to the Excel file where data will be saved.
WAIT_TIME_SECONDS: The time interval (in seconds) between each data fetch.
START_HOUR: The hour (24-hour format) to start fetching data.
END_HOUR: The hour (24-hour format) to stop fetching data.
END_MINUTE: The minute to stop fetching data.
How It Works
Fetching Data:

The script sends a request to the TradingView URL to fetch the HTML content of the page.
Parsing Data:

The HTML content is parsed using BeautifulSoup to extract stock data from the table.
Saving Data:

The extracted data is appended to an Excel file with a timestamp.
Looping:

The script runs a loop that fetches and appends data at regular intervals between the specified start and end times.
Usage
Run the script:

bash
Copy code
python script_name.py
Replace script_name.py with the name of your Python file.

Verify the output:

Check the Excel file specified in FILE_PATH to ensure data is being saved correctly.
Troubleshooting
Failed to fetch data: Ensure that the TradingView URL is correct and accessible.
Excel file issues: Verify that you have write permissions for the specified FILE_PATH.
Contributing
Contributions are welcome! Please fork the repository and submit a pull request with your improvements.

License
This project is licensed under the MIT License.
