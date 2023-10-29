##  **ValueInvestor**




### <u>Background</u>:


We are a portfolio investment company and we make investments in the emerging markets around the world. Our company profits by investing in profitable companies, buying, holding and selling company stocks based on value investing principles.


Our goal is to establish a robust intelligent system to aid our value investing efforts using stock market data. We make investment decisions and based on intrinsic value of companies and do not trade on the basis of daily market volatility. Our profit realization strategy typically involves weekly, monthly and quarterly performance of stocks we buy or hold.


### <u>Goal(s)</u>:

Predict stock price valuations on a daily basis. Recommend BUY, SELL decisions. Maximize capital returns, minimize losses. Ideally a loss should never happen.


### <u>Data Description</u>:


You are given a set of portfolio companies trading data from emerging markets including 2020 Q1-Q2-Q3-Q4 2021 Q1 stock prices. Each company stock is provided in different sheets. Each market's operating days varies based on the country of the company and the market the stocks are exchanged. Use only 2020 data and predict with 2021 Q1 data. Here's the list of 8 companies:
1. Sberbank Rossii PAO(SBER) - Russia.
2. Koc Holding AS (KCHOL) - Turkey.
3. Medinet Masr Housing  - Egypt.
4. Minerva SABrazil - Brazil.
5. Pampa Energia SA - Argentina.
6. Cementos Argos SA - Colombia.
7. Impala Platinum - South Africa.
8. Dongkuk Steel Mil - South Korea.


### <u>Success Metrics</u>:

Evaluate on the basis of capital returns. Use Bollinger Bands to measure your systems effectiveness.

###  <u>Project Overview</u>:
*  The main goal is to predict 2021 stock prices of given portfolio companies using trading data from emerging markets, including 2020 stock price data. Additionally, we aim to recommend Buy, Sell decisions, with a focus on maximizing capital returns and minimizing losses. Our evaluation will be based on capital returns, and we will also utilize Bollinger Bands to gauge our system's effectiveness.
*  The dataset contains 8 different markets from around the world. Each dataset shares the same features: 'Date', 'Price', 'Open', 'High', 'Low', 'Vol.', and 'Change %'. After loading the dataset with the Date as the index, it went through preprocessing steps, which included replacing the variables ('M', 'K', '-') in the 'Change %' column and dividing the 2020 data for training and 2021 for testing. Prepared the time sequence data for model fitting.
*  I applied a univariate LSTM model on the training data, using varying time steps for each dataset and optimizing MSE. After identifying the best MSE, I implemented a trading strategy based on Bollinger Bands to provide Buy and Sell signals. Each unique market achieved positive capital returns without any losses.

### <u>Key Results</u>:
#### Dongkuk Steel Mill's market signals for 2021 were recommended below after prediction :
*  Buy at 8676.28 and Sell at 8642.546
*  Buy at 8397.57 and Sell at 8462.22
*  Buy at 7683.55 and Sell at 8559.57
*  Initial Capital : 100000
*  Final Capital : 111822.42
    ![Korea](https://github.com/skreddypalvai/2EMtf9Oi5Ts8qRbT/assets/137756791/12648009-0f4b-4670-96c8-1f2afa266842)
### Conclusion:
In March, the stock market of all eight companies experienced a downturn due to the impact of the coronavirus pandemic. However, by May, the market had corrected itself, which aligns with the pandemic's timeline. With limited data available, a simple LSTM model was constructed for training. Each individual market exhibited a consistent and decent profit, with no losses incurred.
