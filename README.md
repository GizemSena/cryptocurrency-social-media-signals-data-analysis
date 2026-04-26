🚀 Cryptocurrency + Social Media Signals Analysis
📌 Project Overview

This project analyzes the relationship between cryptocurrency market data and social media signals. The goal is to understand how community engagement, developer activity, and market sentiment influence price movements and market capitalization.

📂 Dataset Description

The dataset contains 2,928 records with the following features:

🪙 Market Data
date: Observation date
coin_id: Cryptocurrency identifier
symbol: Coin symbol
name: Coin name
price_usd: Price in USD
market_cap_usd: Market capitalization
volume_usd: Trading volume
market_cap_rank: Ranking by market cap

📊 Sentiment Data
fear_greed_value: Market sentiment index value
fear_greed_classification: Sentiment category

🌐 Social Signals
wiki_views: Wikipedia page views
reddit_subscribers: Number of Reddit subscribers
reddit_active_users_48h: Active Reddit users
telegram_channel_user_count: Telegram users
github_stars: Github stars
github_forks: Github forks
🔗 Metadata
source_price, source_social, source_wiki, source_sentiment: Data sources
retrieved_at_utc: Data retrieval timestamp

🎯 Objectives
Perform exploratory data analysis (EDA)
Analyze relationships between social signals and crypto prices
Identify patterns in market sentiment and volatility
Build a machine learning model to predict price movement direction

🧹 Data Preprocessing
Converted date columns to datetime format
Removed completely empty columns (e.g., Twitter followers)
Handled missing values using:
Median imputation for numerical features
Zero-filling for sparse social metrics
Encoded categorical variables for modeling

📊 Exploratory Data Analysis
The analysis focused on:

Distribution of price, volume, and market cap
Coin-wise comparisons
Trends over time
Social engagement patterns

🔥 Key Findings from EDA
Increased social activity (Reddit, Github) is associated with higher market activity
Market sentiment (Fear & Greed Index) impacts short-term price fluctuations
Coins with strong developer communities tend to have higher market capitalization
Wikipedia traffic can reflect public interest trends
Trading volume and market cap are strongly correlated

📈 Feature Engineering
New features were created to improve analysis and modeling:

price_change: Daily percentage price change
volatility: Rolling standard deviation (7-day window)
social_score: Combined social engagement metric

🤖 Machine Learning Model
Model Used
Random Forest Classifier
Target Variable
Binary classification:
1 → Price increase
0 → Price decrease
Features Used
Market metrics (market cap, volume)
Sentiment index
Social engagement metrics
Evaluation
Accuracy score used for performance measurement

📊 Feature Importance
The most influential features for predicting price movement:

Market capitalization
Trading volume
Fear & Greed index
Social engagement (Reddit, Github)

🛠️ Technologies Used
Python
Pandas
NumPy
Matplotlib
Seaborn
Scikit-learn

🚀 Future Improvements
Apply advanced models (XGBoost, LightGBM)
Time series forecasting (LSTM, GRU)
Sentiment analysis from Twitter/news data
Real-time crypto prediction system
Trading strategy backtesting

👩‍💻 Author

Gizem Sena Çengel
Computer Engineer
