# Cryptocurrency Trading Bot

## Overview
This project is a Python-based trading bot designed to automate cryptocurrency trading strategies. It fetches market data, applies technical indicators, generates buy/sell signals, and backtests strategies to evaluate performance. The bot incorporates robust risk management features and exports detailed trade metrics for analysis.

## Features
- **Data Fetching**: Fetches OHLCV data from Binance.
- **Technical Indicators**: Calculates MACD, ATR, Bollinger Bands, ADX, and EMAs.
- **Signal Generation**: Generates buy/sell signals based on market conditions.
- **Risk Management**: Implements stop-loss, take-profit, and position sizing.
- **Backtesting**: Simulates strategies on historical data.
- **Performance Metrics**: Tracks win rate, profit factor, Sharpe ratio, and more.
- **Data Export**: Exports trade details and performance metrics to CSV files.

## Results
The bot was backtested on **1,300 days of historical data** for the `BTC/USDT` pair, generating **45 trades** with the following performance metrics:

| Metric               | Value                     |
|----------------------|---------------------------|
| Total Trades         | 45                        |
| Win Rate             | 53.33%                    |
| Profit Factor        | 1.63                      |
| Average Profit       | $1,118.49                 |
| Max Drawdown         | $63,920.75                |
| Sharpe Ratio         | 3.28                      |
| Aggregated Returns   | $50,332.15                |
| Best Trade           | $10,892.78                |
| Worst Trade          | -$10,940.68               |
| Average Holding Time | 3 days, 6 hours           |

## Usage
1. Clone the repository.
2. Install dependencies: `pip install -r requirements.txt`.
3. Update `config.json` with your Binance API keys and parameters.
4. Run the bot: `python main.py`.

## Future Improvements
- Add support for multiple trading pairs.
- Incorporate machine learning models for signal generation.
- Optimize parameters using genetic algorithms or grid search.
- Implement live trading with real-time data.

---

### **Project Insights**

#### **Key Features**
1. **Data Fetching**: Fetches OHLCV (Open, High, Low, Close, Volume) data from Binance using the `ccxt` library.
2. **Technical Indicators**: Calculates indicators like MACD, ATR, Bollinger Bands, ADX, and EMAs to analyze market trends and volatility.
3. **Signal Generation**: Generates buy/sell signals based on a combination of indicators and market conditions (e.g., trend-following and sideways market strategies).
4. **Risk Management**: Implements stop-loss, take-profit levels, and position sizing based on account size and risk tolerance.
5. **Backtesting**: Simulates trading strategies on historical data to evaluate performance metrics like win rate, profit factor, and Sharpe ratio.
6. **Performance Metrics**: Trades are analyzed for profitability, holding time, and risk-adjusted returns.
7. **Data Export**: Exports trade details, signals, and performance metrics to CSV files for further analysis.

#### **Insights from Results**
The bot demonstrated a **positive edge** with a win rate of **53.33%** and a profit factor of **1.63**. Key highlights include:
- **Aggregated Returns**: $50,332.15 over 1,300 days.
- **Risk Management**: Stop-loss and take-profit levels helped mitigate losses during volatile periods.
- **Adaptability**: The bot dynamically adjusts parameters based on market conditions (e.g., trend vs. sideways markets).
- **Scalability**: The modular design allows for easy integration of additional indicators or strategies.

#### **Key Takeaways**
1. **Profitable Strategy**: The bot demonstrated consistent profitability with a strong Sharpe ratio of 3.28.
2. **Risk Management**: Effective use of stop-loss and take-profit levels minimized losses.
3. **Data-Driven Decisions**: Detailed performance metrics and trade exports enable continuous improvement of the strategy.

---

### **Code Overview**
The bot is built using the following Python libraries:
- `ccxt`: For fetching market data from Binance.
- `pandas`: For data manipulation and analysis.
- `numpy`: For numerical calculations.
- `matplotlib`: For visualization (optional).
- `scipy`: For statistical calculations.

#### **Key Components**
1. **DataFetcher**: Fetches and processes OHLCV data.
2. **StrategyEngine**: Implements the trading strategy using technical indicators.
3. **TradeManager**: Manages trades, including backtesting and performance tracking.
4. **TradeSignal**: A data class representing individual trade signals.
5. **Performance Metrics**: Calculates and exports key metrics like win rate, profit factor, and Sharpe ratio.

---

### **Example Performance Metrics Output**
```plaintext
Performance Metrics:
- total_trades: 45
- win_rate: 53.333333333333336
- profit_factor: 1.6286038720554727
- average_profit: 1118.4921522589095
- max_drawdown: 63920.74773172205
- sharpe_ratio: 3.280255576037205
- avg_holding_time: 3 days 06:56:00
- aggregated_returns: 50332.14685165093
- best_trade: 10892.782290584268
- worst_trade: -10940.682150301056
- average_trade_pct: 37.283071741963646
- days_reviewed: 1300
