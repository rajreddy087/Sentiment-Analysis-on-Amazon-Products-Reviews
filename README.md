# Sentiment-Analysis-on-Amazon-Food-Reviews


This project performs sentiment analysis on product reviews using the VADER Sentiment tool and various preprocessing steps to clean and analyze customer feedback. It provides insights into customer sentiments and visualizations of frequent words in both positive and negative reviews.

# Dataset

The dataset contains 1004 product reviews, with the following columns:
- **Id**: Unique identifier for each review
- **ProductId**: Identifier for the product
- **UserId**: Identifier for the user who posted the review
- **ProfileName**: Name of the user
- **HelpfulnessNumerator**: Number of users who found the review helpful
- **HelpfulnessDenominator**: Total number of users who viewed the review
- **Score**: Rating score from 1 to 5
- **Time**: Time the review was posted
- **Summary**: Summary of the review
- **Text**: Full review text

## Preprocessing Steps
1. **Lowercasing**: Converts all text to lowercase.
2. **Punctuation Removal**: Removes all non-alphanumeric characters.
3. **Stopword Removal**: Removes common stopwords (e.g., "and", "the").
4. **Lemmatization**: Reduces words to their base form (e.g., "running" to "run").
5. **Spelling Correction**: Fixes spelling errors in the text.

## Sentiment Analysis
Sentiment analysis is performed using the **VADER Sentiment** library, which categorizes sentiment into:
- **Negative**: Sentiment score for negativity.
- **Neutral**: Sentiment score for neutrality.
- **Positive**: Sentiment score for positivity.
- **Compound**: Overall sentiment score, ranging from -1 (negative) to 1 (positive).

The analysis generates word clouds for both positive and negative reviews, helping to identify common themes and words used by customers in their reviews.

## Insights
- **Most Positive Reviews**: Products with a score of 5 receive the most positive feedback.
- **Most Negative Reviews**: Products with a score of 1 and 2 receive the most negative feedback, which could be valuable for identifying issues with products.
- **Frequent Terms in Reviews**: Wordclouds show the most frequent terms in both positive and negative reviews, offering a quick visual summary of customer sentiments.

## Requirements
- Python 3.x
- Libraries: `pandas`, `matplotlib`, `seaborn`, `nltk`, `textblob`, `vaderSentiment`, `wordcloud`

## Usage
1. Clone this repository.
2. Install the required libraries by running: 
