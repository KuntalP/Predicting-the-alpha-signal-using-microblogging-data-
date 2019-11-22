# Predicting-the-alpha-signal-using-microblogging-data-
The problem consists of a sentiment analysis model and a multiclass classification model. 

# Problem Description
A hedge fund uses 6 financial factors to predict the alpha signal in a stock. This alpha signal is used to make purchase decisions about the stock. The hedge fund now collected and tagged microblogging data for sentiment from the Social Media platform called ‘StockTwits’. 
 
StockTwits is used by people who regularly trade stocks. People on this platform tweet about stocks using the special character ‘$’ to indicate the name of the stock. These microblogs similar to tweets might contain important information about the alpha signal in a stock. 
 
Your goal is to build a sentiment analysis model using the tagged data. This sentiment analysis model should then be used to generate a new stock factor which together with the other stock factors should be used to predict the Alpha Signal. 
 
The hedge fund has anonymyzed the data, which contains 7 stock factors and an alpha signal. This alpha signal is generated using a near perfect algorithmic trading strategy. Unfortunately, the number of stock factors, collected to run that strategy, are extremely high and have to be collected from a large number of data vendors at a high price. 
 
Replicating the alpha signal generated from that strategy using just the 7 Stock Factors and the factor generated from sentiment analysis of the stocktwits would make the company incur significantly less costs to perform their trades. 

# About the data
Two json files: ‘sentiment_train.json’ and ‘sentiment_test.json’ are provided to you which contain stocktwit data, the ‘timestamp’ of collecting the tweet and the ‘ticker’ (stock identifier). The ‘sentiment_train.json’ also contains the tagged sentiment_score ranging from 0 - 3. 
 
There are two csv files provided to you: ‘train_factors.csv’ and ‘test_factors.csv’. The ‘train_factors.csv’ file contains the following fields: 
 
1. Id: Index or unique identifier for a record, in the individual data file. 
 
2. date: The date at which the factors are generated 
 
3. ticker: The identifier through which the company is listed in the stock exchange 
 
4. SF1 - SF7: 7 anonymized Stock Factors that can be used to predict.  
 
5. alpha: The alpha signal generated by using a high performing algorithmic trading strategy. (range: 1 - 4)

# Problem Approach
A) We preprocess the stocktwit_tweets and visualize the data.
B) Build a basic model without sentiment scores (i.e without the json file data)
C) Incorporate the preprocessed tweets to build a multiclass classification model predicting alpha signal.
