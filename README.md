# Movie Recommendation System using Alternating Least Squares (ALS)

This repository contains code for building a movie recommendation system using the Alternating Least Squares (ALS) algorithm. The system is trained on the MovieLens dataset and provides personalized movie recommendations for users.

## Dataset

The MovieLens dataset is used for training and evaluation. It contains movie ratings provided by users.

## Requirements

- Python 3
- NumPy
- SciPy
- Pandas
- Implicit
- Jupyter Notebook (for running the example notebook)

## How ALS Works:

1. Initialize user and item matrices with random values.
2. Alternately optimize the user and item matrices:
   - Fix the item matrix and solve for the user matrix using least squares.
   - Fix the user matrix and solve for the item matrix using least squares.
3. Repeat until convergence or a predefined number of iterations.

ALS is particularly well-suited for implicit feedback datasets, where the absence of an interaction does not necessarily indicate disinterest. It can handle large, sparse datasets efficiently and often provides good recommendations even with limited explicit feedback.

## Example Notebook
The Movie_Recommendation_System.ipynb notebook demonstrates how to:

- Load and preprocess the MovieLens dataset
- Train an ALS recommendation model
- Generate movie recommendations for users
- Evaluate the model's performance

## References
Implicit library: Library for building recommendation systems using collaborative filtering.
MovieLens dataset: Dataset containing movie ratings by users.
