# Twitter Sentiment Analysis

This project uses the Twitter API and the TextBlob library to perform sentiment analysis on tweets related to keywords like "bitcoin" and "cryptocurrency". The tweets and their associated sentiment labels (Positive or Negative) are saved to a CSV file.

## Table of Contents
1. [Installation](#installation)
2. [Usage](#usage)
3. [Data](#data)
4. [Sentiment Analysis](#sentiment-analysis)
5. [Contributing](#contributing)
6. [License](#license)

## Installation

To run this project, you'll need to have the following Python libraries installed:

- `tweepy`
- `pandas`
- `textblob`

You can install these libraries using pip:

```
pip install tweepy pandas textblob
```

You'll also need to provide your own Twitter API credentials, which you can obtain by creating a Twitter Developer account and creating a new application.

## Usage

1. Replace the placeholders `'your_consumer_key'`, `'your_consumer_secret'`, `'your_access_token'`, and `'your_access_token_secret'` in the code with your own Twitter API credentials.
2. Adjust the `keywords` list to search for the topics you're interested in.
3. Run the Python script. The tweets and their sentiment labels will be saved to a CSV file named `twitter_sentiment_analysis.csv`.

```python
python twitter_sentiment_analysis.py
```

## Data

The project uses the Twitter API to search for tweets based on the specified keywords. For each tweet, the following information is collected:

- **Tweet**: The text of the tweet.
- **Sentiment**: The sentiment label, either 'Positive' or 'Negative', based on the sentiment analysis.

The data is then saved to a CSV file named `twitter_sentiment_analysis.csv`.

## Sentiment Analysis

The sentiment analysis is performed using the `TextBlob` library, which provides a simple API for performing basic natural language processing tasks, such as sentiment analysis.

For each tweet, the sentiment polarity is calculated using `TextBlob`. If the polarity is greater than or equal to 0, the sentiment is labeled as 'Positive'; otherwise, it is labeled as 'Negative'.

## Contributing

If you find any issues or have suggestions for improving the project, please feel free to open a new issue or submit a pull request on the project's GitHub repository.

## License

This project is licensed under the [MIT License](LICENSE).
