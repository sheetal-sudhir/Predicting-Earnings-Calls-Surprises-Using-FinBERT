# Predicting-Earnings-Calls-Surprises-Using-FinBERT
This project leverages FinBERT, a BERT-based transformer model, to predict earnings surprises from the earnings call transcripts of NASDAQ-listed companies. The goal is to provide investors with actionable insights into potential market reactions based on earnings call sentiment.

# Dataset 
This project uses earnings call transcripts and financial data from 10 companies (e.g., Apple, Amazon, Google) spanning 2016-2020. The data includes sentiment labels (positive, neutral, negative) indicating earnings surprises, sourced from DataverseNL.

# Methodology
Data Preprocessing: Cleaned transcripts by removing stopwords and punctuation. Sentiments were classified into positive, neutral, or negative based on earnings surprises.

FinBERT Fine-Tuning: Fine-tuned FinBERT for sentiment analysis on the earnings call dataset.

Model Training: Used AdamW optimizer with a learning rate of 5e-5, trained for 5 epochs. Class imbalance was addressed using undersampling.

Evaluation: Model performance was evaluated with accuracy and loss on both balanced and unbalanced data. The model achieved 90% accuracy on unbalanced data.

