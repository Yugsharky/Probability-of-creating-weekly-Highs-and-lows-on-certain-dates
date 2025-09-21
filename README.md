# EUR/USD Weekly High/Low Probability Analysis

A Python script that analyzes historical EUR/USD forex data to determine the statistical probability of each weekday creating weekly highs and lows. This tool helps forex traders and analysts identify patterns in weekly price movements for better market timing and strategy development. You can edit this code for different currencies and timeframes 

## 📊 Features

- **Dual Analysis**: Calculates probabilities for both weekly highs and weekly lows
- **Historical Data**: Fetches real-time EUR/USD data from Yahoo Finance
- **Statistical Insights**: Provides comprehensive probability calculations for each weekday
- **Visual Analysis**: Generates professional 4-chart visualization (bar charts + pie charts)
- **Data Export**: Exports results to CSV for further analysis
- **Flexible Timeframes**: Configurable analysis periods (1y, 2y, 5y, 10y, max)

## 🎯 What It Reveals

The analysis identifies key patterns such as:
- Which days are most likely to create weekly price extremes
- Volatility patterns throughout the trading week  
- Optimal days for different trading strategies
- Market microstructure insights for EUR/USD

## 📈 Sample Results

Based on 5 years of EUR/USD data (2020-2025):

### Weekly Highs Probability:
- **Friday**: 26.9% (Most likely)
- **Monday**: 25.8%
- **Thursday**: 17.7% 
- **Tuesday**: 16.1%
- **Wednesday**: 13.5% (Least likely)

### Weekly Lows Probability:
- **Friday**: 31.1% (Most volatile)
- **Monday**: 28.5%
- **Wednesday**: 16.5%
- **Tuesday**: 12.3%
- **Thursday**: 11.5% (Most bullish)

## 🔧 Installation

### Requirements
```bash
pip install yfinance pandas numpy matplotlib
```

### Dependencies
- `yfinance` - Yahoo Finance API for forex data
- `pandas` - Data manipulation and analysis
- `numpy` - Numerical computations  
- `matplotlib` - Chart generation and visualization

## 🚀 Usage

### Basic Usage
```python
python eurusd_analysis.py
```

### Custom Parameters
```python
# Analyze different time periods
analyzer = WeeklyHighLowProbabilityAnalyzer(period="10y")  # 10 years
analyzer = WeeklyHighLowProbabilityAnalyzer(period="max")  # All available data

# Different currency pairs
analyzer = WeeklyHighLowProbabilityAnalyzer(symbol="GBPUSD=X")  # GBP/USD
analyzer = WeeklyHighLowProbabilityAnalyzer(symbol="USDJPY=X")  # USD/JPY
```

## 📊 Output

The script generates:

1. **Console Output**: Detailed probability tables and key insights
2. **Visual Charts**: 4-panel chart saved as high-resolution PNG
   - Bar chart: Weekly highs probability
   - Pie chart: Distribution of weekly highs  
   - Bar chart: Weekly lows probability
   - Pie chart: Distribution of weekly lows
3. **CSV Export**: Complete data export with timestamps for further analysis

## 📋 Output Files

- `eurusd_analysis_charts_YYYYMMDD_HHMMSS.png` - Visual analysis charts
- `eurusd_weekly_highlow_analysis_YYYYMMDD.csv` - Raw data export

## 💡 Trading Applications

### For Day Traders
- **Timing entries**: Higher probability days for position initiation
- **Volatility plays**: Target Friday/Monday for breakout strategies
- **Risk management**: Adjust position sizes based on expected volatility

### For Swing Traders  
- **Weekly planning**: Anticipate potential weekly extremes
- **Entry optimization**: Thursday entries for bullish setups
- **Exit timing**: Friday profit-taking strategies

### For Analysts
- **Market research**: Understanding EUR/USD weekly cycles
- **Strategy backtesting**: Historical pattern validation
- **Report generation**: Professional charts and statistics

## 🔍 Key Insights Discovered

### High Volatility Days
- **Friday & Monday**: Account for 52.7% of weekly highs and 59.6% of weekly lows
- End-of-week position squaring and start-of-week fresh positioning create volatility

### Most Bullish Day
- **Thursday**: Highest probability for weekly highs, lowest for weekly lows
- Optimal day for long position entries

### Consolidation Period
- **Tuesday-Wednesday**: Lower volatility, suitable for range trading strategies

## 📊 Technical Details

### Data Processing
- Groups daily OHLC data by trading weeks
- Identifies highest high and lowest low for each week
- Calculates statistical frequencies and probabilities
- Filters incomplete weeks (< 3 trading days)

### Statistical Accuracy
- Based on actual historical market data
- Minimum 260 weeks analyzed (5-year default)
- Results validated against multiple timeframes

## ⚠️ Disclaimer

This analysis is based on historical data and should not be considered as financial advice. Past performance does not guarantee future results. Always combine statistical analysis with current market conditions and proper risk management when making trading decisions.

## 🤝 Contributing

Contributions are welcome! Areas for enhancement:
- Additional currency pairs
- Seasonal analysis (monthly/quarterly patterns)  
- Statistical significance testing
- Integration with other technical indicators
- Real-time alerts based on patterns

## 📄 License

This project is open source and available under the MIT License.

## 📞 Support

For questions, issues, or suggestions, please contact me at Halladrian785@gmail.com

<img width="1067" height="893" alt="image" src="https://github.com/user-attachments/assets/c0197ff8-41b1-4911-942b-7fae937df92a" />


