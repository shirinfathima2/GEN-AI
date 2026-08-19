# GEN-AI

AI-Driven Stock News Sentiment Analysis
Project Overview

This project focuses on developing an AI-driven sentiment analysis system to analyze stock-related news and identify its market sentiment. The system uses Natural Language Processing (NLP), text embeddings, Machine Learning, and Neural Networks to classify news articles as positive, neutral, or negative.

The project also explores different text embedding techniques and machine learning models to identify the most effective approach for stock news sentiment classification.

Problem Statement

The increasing number of financial news articles makes it difficult for investors and financial analysts to manually analyze all available information. News and media reports can influence investor perceptions and stock prices.

This project aims to automatically process stock-related news, determine its sentiment, and provide useful insights that can support stock price prediction and investment decision-making.

Dataset

The dataset contains historical daily news and stock market information for a company listed on NASDAQ.

Features
Date – Date on which the news was released.
News – Content of the news article.
Open – Stock price at the beginning of the day.
High – Highest stock price during the day.
Low – Lowest stock price during the day.
Close – Adjusted stock price at the end of the day.
Volume – Number of shares traded during the day.
Label – Sentiment of the news:
1 – Positive
0 – Neutral
-1 – Negative
Objectives
Analyze stock-related financial news.
Perform exploratory data analysis on news and stock prices.
Convert news text into numerical representations using text embeddings.
Classify news into positive, neutral, and negative sentiment.
Compare different embedding techniques.
Compare Random Forest and Neural Network models.
Select an effective model based on classification performance.
Technologies Used
Python
Pandas
NumPy
Matplotlib
Seaborn
Scikit-learn
Gensim
Word2Vec
Sentence Transformers
TensorFlow / Keras
PyTorch
Hugging Face Transformers
Google Colab
Methodology
1. Data Loading

The stock news dataset is loaded into a Pandas DataFrame and basic data inspection is performed.

2. Exploratory Data Analysis

The project analyzes:

Data structure
Missing values
Duplicate values
Sentiment distribution
News length
Monthly stock price trends
Trading volume
Correlation between variables
Relationship between sentiment and stock prices
3. Data Preprocessing

The data is prepared for machine learning by separating the target sentiment labels and splitting the dataset into 80% training and 20% testing data.

4. Text Embeddings

Two major approaches are explored:

Word2Vec

Word2Vec converts individual words into numerical vector representations. The word vectors are averaged to create a representation for each news article.

Sentence Transformers

Sentence Transformer models are used to generate meaningful embeddings for complete news articles. The project explores models such as:

BAAI/bge-base-en-v1.5
all-MiniLM-L6-v2
5. Sentiment Classification

The generated embeddings are used with different classification models:

Random Forest
Neural Network

The models classify news into three sentiment categories: positive, neutral, and negative.

6. Model Evaluation

The models are evaluated using:

Accuracy
Precision
Recall
F1-score
Confusion Matrix

The performance of different combinations of embeddings and models is compared to identify the better-performing approach.

Model Comparison

The project compares the following approaches:

Embedding	Model
Word2Vec	Random Forest
Word2Vec	Neural Network
BAAI/bge-base-en-v1.5	Random Forest
BAAI/bge-base-en-v1.5	Neural Network
all-MiniLM-L6-v2	Random Forest
all-MiniLM-L6-v2	Neural Network
Conclusion

The project demonstrates how NLP and Generative AI techniques can be applied to financial news sentiment analysis. Different text embedding methods and classification models are compared to determine an effective approach for identifying market sentiment from stock-related news.

The analysis shows that the choice of text embedding and classification model can significantly influence sentiment classification performance.

Recommendations / Future Improvements
Use advanced transformer-based models for improved sentiment understanding.
Apply Generative AI to generate summaries of financial news.
Integrate Retrieval-Augmented Generation (RAG) for retrieving relevant financial information.
Combine news sentiment with historical stock prices for better stock prediction.
Develop a real-time system for analyzing newly published financial news.
Build a user-friendly dashboard for financial analysts and investors.
Experiment with larger and more diverse financial datasets.
Project Structure
Project-I-GenAI/
│
├── Project_I_GenAI.ipynb
├── stock_news.csv
└── README.md
