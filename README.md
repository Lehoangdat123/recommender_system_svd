# A Linear Algebra Approach to Machine Learning for Recommender Systems
This project investigates a linear algebra approach, particularly svd matrix factorization, to recommender systems.

## Overview
An iterative SVD-based low-rank approximation algorithm were built to perform matrix completion on a sparse user-item rating matrix. From the completed matrix, the score a user give to an unseen item can be predicted and the top 10 highest rating item can be recommended. Two data-normalization approachs are applied:
- User-based normalization
- Item-based normaliation

The completed matrices are used to compare the rating prediction and recommendation generation ability between two methods.

## Dataset
MovieLens 1M

## Methods
- Data preprocessing
- User-item rating matrix construction
- Matrix completion
- Singular Value Decomposition (SVD)
- Low-rank approximation
- Recommendation generation
- RMSE and MAE evaluation

## Key findings
- Although item-based normalization outperforms in prediction accuracy, user-based normalization provides more personalized recommendation.
- Prediction accuracy does not fully characterize recommendation quality.

## Requirements
Python 3.12
pip install -r requirements.txt

## Run
python src/main.py
