# Sentiment-Analysis
A trading system to take positions on the basis of a sentiment indicator is created.
A backtest is run on microsoft past one-month data. All the related news articles to the company are obtained using newsapi.org
Later polarity and subjectivity are calulated using textblob library. Vader sentiment is also calculated for each of the articles.
An sentiment score indicator is calculated by adding the min and max vader sentiment. 
This indicator takes care of the extremities, say for a particular day we get 2 conflicting news articles, 
one with very positive sentiment and one with a high negative sentiment, we should stay away from such events and not trade.
