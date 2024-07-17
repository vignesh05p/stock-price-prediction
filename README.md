# Stock Prediction App

This Streamlit app predicts stock prices using Facebook's Prophet model. It allows users to select a stock, view its historical data, and see price predictions for the next 1-5 years.

## Features

- Select from a list of stocks
- View historical stock data
- Visualize stock price trends
- Predict future stock prices using Prophet
- Adjust prediction timeframe (1-5 years)

## Prerequisites

Before you begin, ensure you have met the following requirements:

- Python 3.7+
- pip (Python package installer)

## Installation

1. Clone the repository:
   ```
   git clone https://github.com/your-username/stock-prediction-app.git
   cd stock-prediction-app
   ```

2. Create a virtual environment:
   ```
   python -m venv env
   ```

3. Activate the virtual environment:
   - On Windows:
     ```
     .\env\Scripts\activate
     ```
   - On macOS and Linux:
     ```
     source env/bin/activate
     ```

4. Install the required packages:
   ```
   pip install -r requirements.txt
   ```

## Usage

1. Ensure you have a `stock.csv` file in the project directory with at least two columns: "Name" and "Symbol".

2. Run the Streamlit app:
   ```
   streamlit run stock_prediction_app.py
   ```

3. Open your web browser and go to `http://localhost:8501` to view the app.

4. Select a stock from the dropdown menu and adjust the prediction years using the slider.

5. Explore the historical data, prediction graphs, and forecast components.

## Troubleshooting

- If you encounter issues with the `fbprophet` import, try replacing it with `prophet` in the code.
- Ensure you have an active internet connection, as the app fetches real-time stock data.
- If you face any `@st.cache` related warnings, consider updating to `@st.cache_data` for newer Streamlit versions.

## Contributing

Contributions to this project are welcome. Please fork the repository and submit a pull request with your changes.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- [Streamlit](https://streamlit.io/) for the web app framework
- [yfinance](https://github.com/ranaroussi/yfinance) for retrieving stock data
- [Facebook Prophet](https://facebook.github.io/prophet/) for time series forecasting
