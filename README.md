# What Makes a Hit? Predicting BTS Track Popularity

## Overview

This project applies supervised machine learning to predict the popularity of BTS tracks using Spotify audio features and basic metadata.  
Multiple models are compared to assess predictive performance and interpretability, with additional analysis connecting model results to BTS’s musical evolution over time.

## Data

- Spotify audio features (danceability, energy, loudness, speechiness, valence, acousticness, etc.)
- Basic track metadata (release year, album position, duration)
- One observation per track across BTS’s discography
- Data sourced from a pre-collected CSV (no live API calls)

## Methods

- Feature scaling and exploratory data analysis
- Multiple linear regression for directional interpretation
- Random forest regression for non-linear feature importance
- K-nearest neighbors (KNN) for similarity-based prediction
- Train/validation split for model comparison and selection

## Key Findings

- Popularity is driven by combinations of features rather than any single audio characteristic  
- Structural and temporal features (tempo, duration, release year, album placement) show consistent relationships with popularity  
- Highly acoustic or instrumental tracks tend to be less popular within BTS’s catalog  
- Vocal presence and track structure emerge as influential across models  
- Correlated production features affect coefficient interpretation but not overall predictive insight  
- KNN provides a reasonable relative prediction of track popularity (RMSE ≈ 12 on a 0–100 scale)

## Interpretation: BTS’s Musical Journey

- Rap-forward elements appear most effective when balanced with melodic pop structures  
- Production intensity becomes more important as BTS transitions toward global, arena-scale releases  
- Longer tracks and later releases align with BTS’s shift toward fuller, concept-driven albums  
- Acoustic and instrumental tracks play a more niche role compared to vocally driven releases  
- Overall popularity reflects stylistic evolution and balance rather than a single defining sound

## Applications

- Relative comparison of new or unreleased BTS tracks based on audio similarity  
- Insight into how vocal presence, structure, and production relate to popularity  
- Framework that could be extended to multi-artist or genre-level analysis

## Files

- `BTS_Track_Popularity_Prediction.ipynb` — full analysis, modeling, and interpretation

## Tools

Python, pandas, scikit-learn, matplotlib, seaborn

## Notes

This project was developed in Google Colab and uploaded to GitHub for sharing and reproducibility.

## Author

Keelin McLoughlin
