# Music Genre Prediction

## Project Overview

This project explores the relationship between a song’s measurable attributes and its genre, using machine learning techniques to predict music genres based on audio features and popularity data. The motivation stems from the importance of music categorization for streaming platforms, recommendation systems, and the broader music industry.

## Data
- **Source:** [Kaggle - Prediction of music genre](https://www.kaggle.com/datasets/vicsuperman/prediction-of-music-genre?resource=download)
- **Observations:** 50,005 songs
- **Features:** Audio characteristics (danceability, energy, key, loudness, mode, speechiness, acousticness, instrumentalness, liveness, valence, tempo, duration), popularity, and genre (target)

## Data Cleaning
- Removed rows with missing or invalid values (e.g., nulls, non-numeric tempo, non-positive duration)
- Dropped high-entropy and irrelevant columns (e.g., instance_id, obtained_date, track_name)
- Reset dataset indices after cleaning

## Exploratory Data Analysis (EDA)
- Compared feature distributions across genres
- Identified features with high variance by genre: popularity, acousticness, danceability, energy, instrumentalness, speechiness, valence
- Determined less useful features: duration, liveness, loudness, tempo

## Modeling
- Built and evaluated three classification models:
  - Logistic Regression
  - Decision Tree
  - Gaussian Naive Bayes
- Used different feature sets to assess impact on prediction accuracy
- Best model: Logistic Regression (f1-score: 0.50)
- Found that including 'popularity' and high-variance features improved accuracy

## Conclusions
- Audio features and popularity can be used to predict music genre, but accuracy is limited by feature overlap and genre ambiguity
- Logistic Regression outperformed other models in this study
- Further improvements could include better parameter tuning, feature engineering, and deeper exploration of feature relationships

## Team Members
- Caitlyn Li
- Aammya Sapra
- Jackie Wang
- Mishari Almusallam
- Yiting Wang

## License
This project is made available to the public as per the permissions specified in the notebook.
