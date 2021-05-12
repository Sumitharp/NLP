# NLP
## Sentiment Analysis Crypto Currency




## Background

There's been a lot of hype in the news lately about cryptocurrency, so we take stock, of the latest news headlines regarding Bitcoin and Ethereum to get a better feel for the current public sentiment around each coin.

To do this natural language processing is applied to understand the sentiment in the latest news articles featuring Bitcoin and Ethereum. Following tasks are completed : Sentiment Analysis, NLP and Named Entity Recognition.

### 1 - Sentiment Analysis

The [newsapi](https://newsapi.org/) is used to pull the latest news articles for Bitcoin and Ethereum and create a DataFrame of sentiment scores for each coin.

Based on the analysis following questions:

Q: Which coin had the highest mean positive score?

A: Bitcoin has the higher positive mean score of 0.0784 compared to Ethereum's 0.0418

Q: Which coin had the highest compound score?

A: Bitcoin has the highest compound mean score of 0.2844 cf. 0.1205

Q. Which coin had the highest neutral score?

A: Ethereum has the highest neutral score of 0.9489 cf. Btc's 0.9113


### 2 - Natural Language Processing

NLTK and Python is used to tokenize text, find n-gram counts, and create word clouds for both coins. 

#### Tokenize

Tokenized words after:

1. Lowercase each word.
2. Remove punctuation.
3. Remove stop words.

#### N-grams

Next, ngrams and word frequency for each coin.

1. NLTK is used to produce the ngrams for N = 2.
2. List the top 10 words for each coin.

#### Word Clouds

Finally, word clouds is generated for each coin to summarize the news for each coin.

![btc-word-cloud](Images/Bitcoin_wordcloud.png)

![eth-word-cloud](Images/Eth_wordcloud.png)

---

### 3 - Named Entity Recognition

In this section, a named entity recognition model for both coins and visualize the tags using SpaCy.

![btc-ner](Images/btc_ner.png)

![eth-ner](Images/eth_ner.png)

