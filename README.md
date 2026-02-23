# Text Mining: Amazon Fine Foods Reviews

## Overview
This project performs **topic modeling and sentiment analysis** on Amazon Fine Foods reviews.  
Using a sample of 50,000 reviews from the Stanford SNAP dataset, we explore consumer opinion trends, review behavior, and product preference patterns over time.

## Dataset
- Source: [Amazon Fine Foods Reviews Dataset (SNAP)](https://snap.stanford.edu/data/web-FineFoods.html)  
- Sample: 50,000 reviews randomly sampled for analysis  
- Users: 256,059  
- Products: 74,258  
- Period: Oct 1999 – Oct 2012  
- Features: productId, userId, profileName, helpful votes, score, time, summary, text  

## Data Preprocessing
- Parsed raw .txt to structured CSV  
- Lowercased text, removed HTML tags, emojis, punctuation, and short tokens (<3 chars)  
- Removed missing/empty reviews  
- Stopword filtering (NLTK standard + domain-specific)  
- Vocabulary filtering using Gensim (removing extremely rare and overly common words)  
- TF-IDF weighting applied for topic modeling  

## Analysis
- Exploratory analysis: high-frequency words, sentiment distribution, positive vs negative language  
- Topic modeling using **Latent Dirichlet Allocation (LDA)** with 8 topics  
- Topic–sentiment analysis: positive/negative distribution across topics  
- Temporal analysis: topic trends over 1999–2012  
- Behavioral interpretation: insights into habitual consumption and brand loyalty  

## Key Insights
- Beverages and pet food show strong long-term stability, indicating habitual consumption and brand loyalty  
- Sweet and snack products consistently receive high positive sentiment  
- Negative reviews mostly relate to logistics and pricing, not product quality  
- Overall topic distribution is stable over time, despite increasing review volume  

## Repository Structure
- `text_mining_amazon.ipynb` – full preprocessing, topic modeling, and sentiment analysis pipeline  
- `Text Mining Report 2026-02-01.pdf` – detailed project report  

## Tools & Libraries
Python, Pandas, NumPy, NLTK, Gensim, Scikit-learn, Matplotlib/Seaborn, Jupyter/Colab  

## Author
Shan Huang
