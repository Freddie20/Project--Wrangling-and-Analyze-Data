# Project: Wrangling and Analyze Data

This project gather, wrangle and analyze the tweet archive of Twitter user #WeRateDogs which is a Twitter account that rates people’s dogs with funny comments about the dog.

Data gathering
For this project, I gathered the following data on the Twitter Archive File for WeRateDogs:

The Image Prediction TSV file which predicts the dog breeds alongside each tweet ID, image URL, and the image number. This was read into a Jupyter notebook using the Request library and opened using the pd.read_csv function.

The enhanced Twitter archive CSV file which contains basic tweet data of We RateDogs. This file was downloaded and read into the notebook using the pd.read_csv function.

The retweets and favourites count omitted from the enhanced Twitter archive. This file was assessed programmatically using the Tweepy library to query Twitter's API. To get just the tweet id, retweets and favourites count:
- I defined dictionaries to hold key-value pairs of tweet_id and retweet count and tweet_id and favourite count
- I used a loop to try-except-else to test API connection, show error, or else fill the corresponding dictionary with required retweet and favourite, count values.
