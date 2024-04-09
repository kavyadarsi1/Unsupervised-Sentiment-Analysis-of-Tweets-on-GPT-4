# Unsupervised Sentiment Analysis of Tweets on GPT-4

## Project Overview
This project explores the application of unsupervised learning techniques for sentiment analysis of Twitter data concerning public opinion on GPT-4. Utilizing K-means clustering, this project categorizes tweets into positive, negative, or neutral sentiments, offering insights into societal perspectives on GPT-4 without the need for labeled data.


## Introduction
Our project aims to capture the sentiment toward GPT-4, a potential successor to GPT-3, by analyzing tweets using the K-means clustering algorithm. Through this analysis, we seek to understand the complex and nuanced language expressions on social media regarding GPT-4.

## Technologies Used
- Data Collection: Twitter API, Kaggle
- Data Preprocessing: Python (Pandas, NumPy), Regular Expressions
- NLP: Tokenization, Lemmatization, Word2Vec
- Clustering Algorithm: K-means
- Model Evaluation: Cohen's Kappa Score
- Visualization: Matplotlib, Word Cloud
- Benchmarking Models: BERT, VADER

## Dataset
The dataset comprises around 28,000 tweets related to GPT-4, with the final analytical dataset containing 20,465 tweets after cleaning and preprocessing. Sentiments were scored from -1 (negative) to 1 (positive) based on the textual polarity.

## Methodology
Data Preprocessing
Involved removal of spam, duplicates, and irrelevant characters, conversion of text to lowercase, and tokenization into meaningful units.

## Modeling
The project employed Word2Vec for generating embeddings and K-Means for clustering tweets into sentiment categories, later manually labeled as positive, negative, or neutral.

## Evaluation
Cohen's Kappa Score was used for evaluation, indicating the level of agreement between our model's sentiment assignments and those from BERT, VADER models, and human assessments.

## Key Findings and Numerical Values
- The K-Means model distribution showed a majority of words clustered in negative and neutral sentiments, indicating a significant public discourse on these aspects concerning GPT-4.
- Cohen’s Kappa Score between K-Means model vs. BERT and VADER models:
  - BERT: -0.153846
  - VADER: 0.037736
- The comparison with human benchmarks yielded scores ranging from -0.045455 to 0.062500, revealing varied levels of agreement and highlighting the subjective nature of sentiment analysis.
- The distribution of sentiment according to BERT and VADER models suggested differing perspectives on the sentiment prevalent within the dataset, with BERT finding a near-even distribution between positive and negative sentiments.

## Conclusion
This project provided valuable insights into the application of unsupervised learning for sentiment analysis on Twitter. Despite the challenges in achieving high accuracy due to the nuanced language used in tweets, our findings offer a foundational understanding of public sentiment towards GPT-4. Future directions include enhancing data preprocessing and exploring advanced clustering techniques to improve the model's accuracy and reliability.

## References
- Agashini V Kumar, Meera K. N. (2022) Sentiment Analysis Using K Means Clustering on Microblogging Data Focused on Only the Important Sentiments. ICETET-SIP-22
- Pierre Megret (2018). Gensim Word2Vec Tutorial.
- Rafał Wójcik (2019). Unsupervised Sentiment Analysis.
- Kurtis Pykes (2020). Understanding Cohen’s Kappa coefficient.
- Mary L. McHugh (2012). Interrater reliability: the kappa statistic.
