# Sentimental Tomatoes: Leveraging Feature Engineering and ML for Rotten Tomatoes Sentiment Prediction

***The complete notebook featuring the entire process outlined below can be seen [here](https://github.com/XiongCynthia/ML-with-Sentimental-Tomatoes/blob/main/Sentimental_Tomatoes.ipynb).***

---

## Overview

We have performed feature engineering and logistic regression/naïve bayes ML models to predict sentiments of movie reviews.

The dataset is comprised of tab-separated files with sentences and phrases from the Rotten Tomatoes dataset. Phrases and sentences have been parsed by the Stanford parser, and each phrase and sentence have their own IDs. Multiple phrases can belong to the same sentence. Phrases that are repeated (which are typically short or common single words) are only included once in the each of the datasets.

Each phrase/sentence in the training data are labelled with one of the five sentiment scores:
- 0 - negative
- 1 - somewhat negative
- 2 - neutral
- 3 - somewhat positive
- 4 - positive

Our objective is to predict the sentiment of movie review sentences and phrases from the testing data with as much accuracy as possible.

Source: [https://www.kaggle.com/competitions/sentiment-analysis-on-movie-reviews/overview](https://www.kaggle.com/competitions/sentiment-analysis-on-movie-reviews/overview)

---

## Summary of the Process

1. Exploratory data analysis
    - Compare the assigned sentiment scores of sentences vs. phrases
    - Create word clouds of all sentences
    
2. Feature engineering (and more EDA)
    - Vectorize sentences into TF-IDF values
    - Polarity (sentiment strength) scores
    - Subjectivity scores
    - Part of speech (POS) tag counts
    - Phrase/sentence lengths
    - Counts of '!', '?', and '.'
      
3. Train naïve Bayes and logistic regression models
      
4. Evaluate models
    - Compare mean accuracy scores
    - Compare precision, F1, and recall scores
    - Perform k-fold cross-validation
    - Evaluate features' contribution to the model

5. Choose best model for final predictions
    - Save results in a csv and submit to Kaggle
