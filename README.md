# Stock Prediction using LSTM

For this project, we focused on predicting stock prices with the integration of sentiment analysis. The rationale behind this approach is that news, tweets, and social media activity significantly influence the movement of a company's stock price. By incorporating sentiment analysis, we aim to capture these external factors to enhance the accuracy of our predictions.

We selected **Apple Inc. (AAPL)** as the stock of interest. We also found an open-source dataset accumulating sentiments for different stocks over a period of 365 days i.e. \(2019 - 2020). https://github.com/adlnlp/StockEmotions?utm_source=chatgpt.com

## Approaches
We explored some distinct approaches for this project:

1. **Stock Price Prediction Using Time-Series**

  Using historical stock price data to predict future prices using time-series modeling.

1. **Stock Price Prediction Using LSTM \(Without Sentiment Analysis)**  
   Using historical stock price data alone to predict future prices.

2. **Stock Price Prediction Using LSTM \(With Sentiment Analysis)**  
   Combining historical stock data with sentiment scores derived from news and social media to potentially improve predictions.

## Methodology

For both latter approaches, we utilized a Long Short-Term Memory (LSTM) neural network. We first used a normal LSTM but then improved upon it and got better results.

## Steps
1. **Data Collection**:
   - Historical stock price data for AAPL.
   - Sentiment data derived from news articles, tweets, and social media posts related to Apple.

2. **Data Preprocessing**:
   - Normalizing stock price data for LSTM input.
   - Assigning sentiment scores for either a Bullish or a Bearish trend.

3. **Model Training**:
   - Training a normal sequential model using time-series modeling.
   - Training the LSTM model on historical stock data for the second approach.
   - Incorporating sentiment scores alongside stock data for the third approach.

4. **Evaluation**:
   - Comparing the performance of the three models to assess the impact of sentiment analysis on prediction accuracy.

