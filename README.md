# Stock Price Prediction Using Twitter Sentiment Analysis
## Project Overview
This project combines financial market data with Twitter sentiment analysis to predict stock prices using Generative Adversarial Networks (GANs). It aims to uncover how public opinion on social media impacts stock movements and leverage that insight to enhance price forecasting accuracy.

## Business Problem
Stock prices are highly influenced by market sentiment, news, and public perception—especially in real-time environments like Twitter. The goal of this project is to predict stock prices more effectively by incorporating real-time tweet sentiment data, enabling investors, analysts, and financial institutions to make better-informed decisions.

## Tools, Techniques & Workflow
* Data Collection:
  * Historical stock price data (Yahoo Finance)
  * Tweets related to the stock using Twitter API

* Preprocessing:
  * Tweets cleaned and labelled using VADER Sentiment Analysis
  * Stock data scaled and aligned with sentiment scores
  * Train/Test split with proper index tracking

* Model Architecture:
  * Built a Generative Adversarial Network (GAN) comprising:
    * Generator: Predicts future stock prices
    * Discriminator: Differentiates real vs generated prices
  * Used LSTM layers for sequence modelling
  * Implemented using TensorFlow / Keras

* Process:
  1. Clean & merge tweet and stock data
  2. Generate sentiment features
  3. Train GAN model on combined dataset
  4. Evaluate performance using RMSE and visual comparison

## Results & Business Impact
* The GAN model was able to learn the underlying patterns in price movements with a test RMSE of 13.5, indicating promising predictive power.
* The model captures market sentiment fluctuations from tweets, providing a more realistic and reactive forecast than models based solely on historical prices.
* Potential use cases:
  * Real-time stock alerts for traders
  * Sentiment-aware investment strategies
  * Risk mitigation tools for financial advisors

## Conclusion
This project shows that combining NLP-driven sentiment analysis with deep learning models like GANs can yield more insightful and accurate stock predictions. It bridges the gap between quantitative data and human emotions, highlighting the importance of alternative data sources in financial analytics.
