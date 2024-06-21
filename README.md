# Amazon Consumer Reviews Analysis

## Project Overview
Amazon receives billions of consumer reviews every day. This project aims to analyze a dataset of these consumer reviews to identify common themes and sentiments. By understanding the sentiments expressed in these reviews, we can uncover the most frequently mentioned issues faced by consumers.

## Objectives
- **Theme Extraction**: Identify recurring themes and topics within the reviews.
- **Sentiment Analysis**: Determine the sentiment of the reviews, categorizing them as positive, negative, or neutral.
- **Problem Identification**: Highlight the most common problems mentioned by consumers in their reviews.

## Data and Preprocessing

### Data Source
The dataset consists of consumer reviews collected from Amazon.

### Data Cleaning
- **Text Cleaning**: Remove special characters, single characters, and multiple spaces. Convert text to lowercase.
- **Stopwords Removal**: Eliminate common stopwords to focus on meaningful words.
- **Tokenization**: Split text into individual words (tokens) and sentences.
- **Lemmatization**: Convert words to their base forms for consistency.

### Libraries Used
- **Data Handling**: `pandas`
- **NLP and Sentiment Analysis**: `nltk`, `spacy`, `fast_bert`, `pytorch_transformers`
- **Visualization**: `matplotlib`, `WordCloud`

## Methodology

### Sentiment Analysis
Using the VADER sentiment analysis tool from the `nltk` library, we calculate sentiment scores for each review. The scores help in categorizing the sentiment of the reviews into positive, negative, or neutral.

### Theme Extraction
We use tokenization and part-of-speech tagging to identify key themes and topics in the reviews. This involves categorizing words into nouns, verbs, adjectives, etc., and analyzing their frequency.


- **PyATE**: Implemented term extraction using algorithms such as C-Value, Basic, Combo Basic, Weirdness, and Term Extractor with spaCy POS tagging.
- **Batch Processing**: Data was processed in batches to efficiently handle large datasets and loaded into a processed table for further analysis.
- **Term Restructuring**: Extracted terms and their scores were restructured into a single column format for easier analysis.


### Data Visualization
To visualize the results, we create word clouds and frequency distribution plots. These visualizations help in understanding the most common words and themes in the reviews.

## Results
- **Top Themes**: The analysis reveals the most frequently mentioned themes in the reviews, such as product quality, price, and customer service.
- **Sentiment Distribution**: The sentiment analysis provides an overview of the proportion of positive, negative, and neutral reviews.
- **Common Problems**: By focusing on negative reviews, we identify the most common problems faced by consumers, such as product defects and poor customer service.

## Conclusion
This project provides valuable insights into consumer sentiments and recurring themes in Amazon reviews. By understanding these aspects, businesses can improve their products and services to better meet customer needs.

## Future Work
- **Deep Learning Models**: Implement advanced deep learning models for more accurate sentiment analysis.
- **Topic Modeling**: Use topic modeling techniques to uncover hidden patterns and topics in the reviews.
- **Extended Analysis**: Analyze reviews from different product categories separately for more targeted insights.

## Dependencies
- `pandas`
- `pytorch_transformers`
- `fast_bert`
- `spacy`
- `nltk`
- `matplotlib`
- `WordCloud`
