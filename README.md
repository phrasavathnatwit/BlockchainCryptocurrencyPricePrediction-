# Blockchain: Cryptocurrency Price Prediction 

This project applies data science and machine learning techniques to explore and predict short-term price movements of major cryptocurrencies—specifically Bitcoin (BTC) and Ethereum (ETH). It aims to uncover key market indicators that influence price changes, compare volatility across assets, and assess the effect of external events such as regulatory news and social media sentiment on the crypto market.

---

## Abstract
This project explores the feasibility of predicting short-term cryptocurrency price changes—specifically Bitcoin and Ethereum—using various machine learning models such as LSTM, ARIMA, and XGBoost. The goal is to analyze which factors influence price movements and assess how accurately price trends can be forecasted within a 24-hour window. Through the use of historical data, social sentiment, and external market indicators, this study aims to contribute to the growing field of crypto analytics.

Keywords: Cryptocurrency, Machine Learning, Price Prediction, Bitcoin, Ethereum, Time Series Analysis, LSTM, ARIMA, XGBoost

---

## Project Objectives
 
The core of this project is structured around four key research questions:

1. **What market factors (e.g., trends, volume) have the strongest correlation with cryptocurrency price changes?**
2. **How accurately can a machine learning model predict the price of Bitcoin or Ethereum for the next 24 hours?**
3. **How does the volatility of Bitcoin compare with other cryptocurrencies over time?**
4. **How do significant spikes in trading volume or sudden price changes impact short-term movements of Bitcoin and Ethereum?**

---

## Datasets Used

The project utilizes four main datasets:

1. **[BTC & ETH 1-Minute Price History (Kaggle)](https://www.kaggle.com/datasets/patrickgendotti/btc-and-eth-1min-price-history)**  
   High-resolution minute-by-minute price data from 2014 onward.  
   Includes: `Timestamp`, `Open`, `High`, `Low`, `Close`, `Volume`

2. **[CryptoDataDownload](https://www.cryptodatadownload.com/)**  
   OHLC and volume data at daily, hourly, and minute intervals across major exchanges.

3. **[Yahoo Finance ETH-BTC Historical Data](https://finance.yahoo.com/quote/ETH-BTC/history/)**  
   Daily exchange rate data between ETH and BTC for volatility and valuation comparison.

4. **[Crypto News+ Dataset (Kaggle)](https://www.kaggle.com/datasets/oliviervha/crypto-news)**  
   Over 280,000 news articles labeled with sentiment (Positive, Neutral, Negative).  
   Used to assess the impact of external events on price fluctuations.

---

## Methods and Tools

- **Languages**: Python (Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn, TensorFlow/Keras)
- **Models**: LSTM (Long Short-Term Memory), ARIMA, XGBoost, Random Forest Regressor
- **Evaluation Metrics**: MAE, RMSE
- **Feature Engineering**:
  - Rolling volatility
  - Price change %
  - Moving averages (MA-10, MA-30)
  - Sentiment averaging
  - External event flags

---

## Results
After training and testing each model, we found the following:

XGBoost achieved the most consistent short-term accuracy on test data with relatively fast training times.

ARIMA worked well for linear trends but struggled with high volatility periods.

LSTM, while powerful, required more tuning and data preparation to outperform the other models.

Notably, social sentiment data (Twitter and Reddit) showed measurable correlation with price surges, especially for Bitcoin. However, sentiment-based models alone were insufficient without historical price context.

These results highlight the importance of hybrid modeling—combining historical technicals with real-time social indicators—to improve crypto price forecasting.

---

## Future Work
Model Optimization: Further tuning of hyperparameters, especially for LSTM and XGBoost models, could improve prediction accuracy.

Multi-Crypto Prediction: Expanding beyond Bitcoin and Ethereum to include other coins like Solana or Ripple may reveal more diverse insights.

Real-Time Prediction: Implementing a live price prediction dashboard using APIs from platforms like Binance or CoinGecko.

Sentiment Analysis Expansion: Incorporate more advanced NLP techniques (e.g., BERT) to process social media sentiment more accurately.

Integration of Macroeconomic Factors: Adding indicators such as interest rates, inflation, or regulatory news could enhance model performance.

---

## Conclusion
This project demonstrates that machine learning models, particularly XGBoost and LSTM, hold potential for forecasting short-term cryptocurrency price movements. While historical data remains a strong predictor, incorporating external factors like sentiment adds valuable context. The findings suggest that a multi-input approach combining technical, social, and external data sources is more effective than relying on a single stream. These results can serve as a stepping stone for building more sophisticated prediction tools and offer practical insights for traders, analysts, and researchers in the crypto space.

