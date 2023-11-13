# Sentimental Tomatoes: Leveraging Feature Engineering and ML for Rotten Tomatoes Sentiment Prediction

We will be performing feature engineering and logistic regression/naive bayes ML models to predict sentiments of movie reviews.

The dataset is comprised of tab-separated files with sentences and phrases from the Rotten Tomatoes dataset. Phrases and sentences have been parsed by the Stanford parser, and each phrase and sentence have their own IDs. Multiple phrases can belong to the same sentence. Phrases that are repeated (which are typically short or common single words) are only included once in the each of the datasets.

Each phrase/sentence in the training data are labelled with one of the five sentiment scores:
- 0 - negative
- 1 - somewhat negative
- 2 - neutral
- 3 - somewhat positive
- 4 - positive

Our objective is to predict the sentiment of movie review sentences and phrases from the testing data with as much accuracy as possible.

Source: [https://www.kaggle.com/competitions/sentiment-analysis-on-movie-reviews/overview](https://www.kaggle.com/competitions/sentiment-analysis-on-movie-reviews/overview)
