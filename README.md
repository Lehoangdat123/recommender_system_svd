# A Linear Algebra Approach to Machine Learning for Recommender Systems
This project investigates a linear algebra approach, particularly SVD matrix factorization, to recommender systems.

## Overview
An iterative SVD-based low-rank approximation algorithm was built to perform matrix completion on a sparse user-item rating matrix. From the completed matrix, the score a user gives to an unseen item can be predicted and the top 10 highest-rated items can be recommended. Two data-normalization approaches are applied:
- User-based normalization
- Item-based normalization

The completed matrices are used to compare the rating prediction and recommendation generation ability between the two methods.

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
- Although item-based normalization outperforms in prediction accuracy, user-based normalization provides more personalized recommendations.
- Prediction accuracy does not fully characterize recommendation quality.

## Requirements
Python 3.12
pip install -r requirements.txt

## Run
The project is implemented in a Jupyter Notebook and was developed and tested using Google Colab.

1. Open the notebook
Open the notebook located in the notebooks/ folder:

notebooks/svd_recommender.ipynb

You can either download the notebook and upload it to Google Colab or open it directly from the GitHub repository using Open in Colab.

3. Install the required libraries

If necessary, run the following cell at the beginning of the notebook:

!pip install -r requirements.txt
3. Run the notebook

Run the notebook cells from top to bottom:

Runtime → Run all

Alternatively, execute each cell individually using the ▶ button.

The notebook will:

Load the MovieLens dataset.
Preprocess the rating data.
Construct the user-item rating matrix.
Apply Singular Value Decomposition (SVD).
Perform matrix completion and prediction.
Evaluate the predictions using RMSE and MAE.
Generate movie recommendations.
