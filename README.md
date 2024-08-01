# Stock Trend Prediction
## Predicting Stock Market Trends Using News Sentiment Analysis and Machine Learning Models (LSTM, ARIMA, and Linear Regression)

## Introduction 
Incorporating extracted news headlines with historical data, this project showcases a complete process to predicting stock market trends. The central hypothesis is that the sentiment reflected in headlines and articles can provide valuable insights into market behaviour, influencing investor outlooks and, consequently, stock prices.

Integral to this analysis is the Random Walk Theory, developed by Charles Dow and later popularized by Burton Malkiel. Their studies suggest that stock prices move randomly and that predicting future movements based on historical data is inherently challenging. Thus, rather than forecasting exact prices, this project focuses on uncovering broader market trends and movements by incorporating news sentiments. 

The project begins by obtaining historical stock data from Yahoo! Finance using the "yfinance" API and news data from News API. It proceeds with the visualization of relevant news authors and sources, as well as historical close prices and Open-High-Low-Close (OHLC) data. To analyze these trends, machine learning models such as Long Short Term Memory (LSTM), Autoregressive Integrated Moving Averages (ARIMA), and Linear Regression are utilized. Lastly, the accuracy of these models is validated through metrics such as Mean Squared Error (MSE), mean MSE, Root Mean Squared Error (RMSE), and visual line plots. 

The following section further explores the reasoning behind the chosen algorithms: 

### Long Short-Term Memory (LSTM): 

According to NVIDIA developers, an LSTM is a Recurrent Neural Network (RNN) designed to prevent issues with the input flowing through feedback loops. These feedback loops are key to better-recognizing patterns by selecting and discarding information to make room for new memory. Therefore, LSTMs are ideal for "solving sequence learning tasks," such as language text analysis. 

###  Autoregressive Integrated Moving Averages (ARIMA): 

ARIMA is widely used to forecast future stock prices based on historical time series. The model looks at the most ideal pattern in the unit of time, which is 30 days in this project, and uses aggregate sentiment and stock price values for prediction.

### Linear Regression: 

This statistical model establishes a linear relationship between the dependent variable (stock prices) and one or more independent variables (historical prices and sentiment scores), providing a straightforward method for predicting future values based on these relationships.


## Objectives and Step-by-step process: 

1. Data Collection: Compile historical stock data and relevant news articles.

2. Sentiment Analysis: Extract and quantify sentiment from news headlines to gauge the general market attitudes and their potential impact on stock trends.

3. Feature Engineering: Develop data frames that capture features which combine sentiment scores with historical stock data. 

4. Model Development and Evaluation: Build and train models forecasting the overall market trend, and evaluate model performance using metrics assessing accurate market direction predictions. 

### Libraries and Documentation: 

The following Python libraries and APIs are used in this project: 

- pandas
- numpy
- datetime 
- json_normalize
- matplotlib
- seaborn
- plotly
- newsapi-python
- yfinance
- mplfinance
- nltk
- vaderSentiment
- textblob
- regex
- scikit-learn
- scipy
- tensorflow
- keras
- pmdarima
- statsmodels

References and sources: 
- http://www.stat.yale.edu/Courses/1997-98/101/linreg.htm
- https://developer.nvidia.com/discover/lstm
- https://www.jatit.org/volumes/Vol100No4/23Vol100No4.pdf
- https://www.ibm.com/topics/arima-model
