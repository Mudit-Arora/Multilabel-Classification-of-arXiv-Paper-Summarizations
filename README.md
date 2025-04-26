# Multilabel-Classification-of-arXiv-Paper-Summarizations
For this task, I processed the data, did feature engineering, and trained different models to predict which category (or categories) an arXiv paper’s abstract belongs in.

### Results
1. Best performing model: Random Forest wrapped in OneVsRestClassifier
2. Data preprocessing included: conversion of lowercase, removal of special characters, removal of stopwords, lemmatization using NLTK's WordNetLemmatizer, and filtering out words with length <= 2
3. Features:
- Summary Length: word count of each summary 
- BoW: captures technical terminology frequency 
- TFIDF: weights domain-specific terms higher, reduces the impact of common academic words
4. Micro F1 Score on Validation Set: 0.79
Macro F1 Score on Validation Set: 0.35
Micro F1 Score on Test Set: 0.79
Macro F1 Score on Test Set: 0.35
