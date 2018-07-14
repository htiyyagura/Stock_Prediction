# Dataset
Dataset consists of following files:

prices.csv: raw, as-is daily prices. Most of data spans from 2010 to the end 2016, for companies new on stock market date range is shorter. There have been approx. 140 stock splits in that time, this set doesn't account for that.

prices-split-adjusted.csv: same as prices, but there have been added adjustments for splits.

securities.csv: general description of each company with division on sectors

fundamentals.csv: metrics extracted from annual SEC 10K fillings (2012-2016), should be enough to derive most of popular fundamental indicators.

# What we are going to do
An evnet driven model that uses financial time series data, technical indicators and New York Times headlines to form a Gated Recurrent Unit neural network.

# How ?
1. Download the news from NY Times.
2. Combine news and technical data.
3. Data preparation and sentiment analysis.
4. Predict using Recurrent Neural Network
5. Adding twitter sentiment to the data (if time permits)
