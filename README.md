# Blockchain: Cryptocurrency Price Prediction 

This project applies data science and machine learning techniques to explore and predict short-term price movements of major cryptocurrencies—specifically Bitcoin (BTC) and Ethereum (ETH). It aims to uncover key market indicators that influence price changes, compare volatility across assets, and assess the effect of external events such as regulatory news and social media sentiment on the crypto market.

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
- **Evaluation Metrics**: MAE, RMSE, R²
- **Feature Engineering**:
  - Rolling volatility
  - Price change %
  - Moving averages (MA-10, MA-30)
  - Sentiment averaging
  - External event flags

---

