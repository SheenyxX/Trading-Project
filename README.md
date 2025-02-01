
# Cryptocurrency Analysis Tool: BTC/USDT

This Python script helps traders make **better-informed decisions** by analyzing BTC/USDT trading data. It calculates key indicators like **MACD** and **volume trends**, providing insights into the trading environment. The script fetches data from Binance, processes it, and generates visualizations to help you understand market conditions.

---

## **What Does This Code Do?**
1. **Fetches Data**:
   - Gets BTC/USDT trading data (price and volume) from Binance.

2. **Analyzes Volume**:
   - Classifies volume into 5 tiers (Very Low, Low, Moderate, High, Very High) based on historical data.
   - Helps you understand whether trading activity is high or low.

3. **Calculates MACD**:
   - Computes the **Moving Average Convergence Divergence (MACD)** indicator, which helps identify trends and potential buy/sell signals.

4. **Generates Visualizations**:
   - **Price Trends**: Shows how the price has moved over the last 30 and 90 days.
   - **MACD Plots**: Displays MACD, Signal Line, and Histogram to highlight trends.
   - **Volume Analysis**: Visualizes volume trends with color-coded bars and donut charts.

5. **Provides Insights**:
   - Detects MACD crossovers and divergences, which are key signals for trading decisions.
   - Checks data quality to ensure the analysis is based on reliable data.

---

## **How Does This Help with Trading?**
- **Volume Analysis**: Helps you understand market activity. For example, high volume often indicates strong interest in the asset.
- **MACD Signals**: Identifies potential buy/sell opportunities based on trend changes.
- **Visualizations**: Makes it easy to spot patterns and trends in price and volume.

By combining these insights, you can make **better-informed trading decisions** based on data rather than guesswork.

---

## **Requirements**
To run this script, you need the following Python libraries:
- `ccxt`
- `pandas`
- `numpy`
- `matplotlib`
- `seaborn`

Install the dependencies using:
```bash
pip install ccxt pandas numpy matplotlib seaborn
```

---

---

## **Customization**
- **Symbol**: Change the `symbol` variable in the `main()` function to analyze other trading pairs (e.g., `ETH/USDT`).
- **Timeframe**: Modify the `timeframe` variable to fetch data for different intervals (e.g., `1h`, `4h`).
- **Thresholds**: Adjust the `THRESHOLDS` list to change volume classification percentiles.

---

## **Contributing**
Contributions are welcome! If you find any issues or have suggestions for improvement, please open an issue or submit a pull request.

---

---

## **Author**
[Andrew R]  
[github.com/SheenyxX ]  

