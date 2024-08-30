# SEC Document Scraper & Stock Price Predictor for NVDA

This repository contains a Python-based tool that scrapes 10k financial documents from the SEC website and analyzes them to predict stock price movements for NVIDIA Corporation (NVDA). Using natural language processing techniques like cosine and Jaccard similarity, the tool evaluates the textual content of these documents to identify patterns and correlations that could indicate future stock performance.

### Key Features:
- Data Scraping: Efficiently scrape 10-K documents from the SEC EDGAR Database for multiple publicly traded companies. Perform thorough data cleaning, including removing HTML tags and numerical tables, converting documents to plain text, lemmatization, stemming, and removing stop words to prepare for text analysis.
- Exploratory Data Analysis (EDA): Analyze textual data from 10-K documents using techniques such as Bag of Words (BoW), TF-IDF, Wordclouds, Latent Dirichlet Allocation (LDA) modeling with interactive pyLDAvis, and TextBlob for sentiment analysis (positivity score).
- Text Similarity Analysis: Calculate cosine and Jaccard similarity scores between consecutive 10-K documents for each firm, focusing on computational efficiency. Evaluate the differences in similarity scores year over year to understand changes in document content.
- Stock Price Correlation: Map text changes identified through similarity scores with historical stock price movements. Download stock prices from the date of the first available 10-K document to the filing date of the most recent one. Analyze and compare the results to determine if textual changes align with stock price movements.
- Hypothesis Testing: Conclude whether the analysis supports that textual changes in 10-K documents correlate with stock price movements.
