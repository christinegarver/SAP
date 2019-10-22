# Tweet Sentiment-Analysis Platform

Using logistic regression, I created a model that classifies a tweet as happy or sad. The model identified the test set with an accuracy greater than 50%.

Before training the model, I cleaned the data. I made sure to remove stop words and punctuation marks.

Due to limited space on my computer, I had to one-hot encode each tweet example one-by-one as the model processed the batches, instead of one-hot-encoding all the examples at once before trianing the model. However, the matrix does account for every word in all examples - it is 1 x n (n = # of unique words in all examples).

I do not think this tweet sentiment analysis platform is perfect, but it is my first draft. I will continue to work on it to increase accuracy score.

I think one issue with my model is that in order to mark a tweet as happy or sad, the model must process and parse the tweet. This is because I processed all the data before splitting the data into training, testing, and validation sets. In the real world, if my model was given a tweet, I would have to process and parse the tweet.

After increasing the accuracy of my model, I will make a function or command line application where one can just feed in the tweets unprocessed in order to be classified as happy or sad.

## Built with

- Python
- PyTorch

## Authors

Christine Garver

## Acknowledgements

Used data from: http://help.sentiment140.com/for-students
