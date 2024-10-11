# Recommender Systems Project - Beer Ratings and Recommendations

## Overview

This project was completed as part of the Recommender Systems course during the second semester of 2024. The objective of the task was to apply different recommendation algorithms to predict user ratings and generate personalized recommendation lists. The project was divided into two main parts: rating prediction and ranking generation.

## Objectives

1. **Rating Prediction**: Complete the missing ratings in the provided `.csv` file by predicting the user’s evaluation of different beers.
2. **Recommendation List Generation**: Generate a list of the top 10 beer recommendations for each user in the provided `.json` file.
3. **Model Evaluation**: Evaluate and compare the results using metrics such as RMSE for rating prediction and Recall@10, nDCG@10, and MAP@10 for recommendation quality. Additionally, measure the diversity and novelty of the generated recommendations.

## Dataset

The datasets used in this project include:

- **Training Set (`training_set.csv`)**: 35,534 records from 8,320 users, each providing a rating for a particular beer.
- **Validation Set (`validation_set.csv`)**: 8,845 records from 3,410 users for validation purposes.
- **Rating Test Set (`rating_template_fill.csv`)**: 2,945 records requiring rating predictions.
- **Ranking Test Set (`ranking_template_fill.json`)**: 1,953 keys requiring top 10 recommendations per user.

## Algorithms

For this task, the following algorithms were applied:

### Part 1: Rating Prediction

- **User-based Collaborative Filtering**
- **Item-based Collaborative Filtering**
- **FunkSVD**
- **SVD++ (optional)**

### Part 2: Recommendation List Generation

- **Item-based Collaborative Filtering**
- **FunkSVD**
- **Alternating Least Squares (ALS)**
- **Bayesian Personalized Ranking (BPR)**
- **Factorization Machines**

## Evaluation Metrics

The performance of the models was evaluated using the following metrics:

- **Rating Prediction**: RMSE (Root Mean Squared Error)
- **Ranking Generation**:

  - **Recall@10**
  - **nDCG@10** (Normalized Discounted Cumulative Gain)
  - **MAP@10** (Mean Average Precision)
- **Diversity**: The average number of distinct beer styles recommended.
- **Novelty**: Measured by the self-information of the recommended items.

## Results

The results were evaluated on the validation set. A detailed analysis of each method's performance, including the **RMSE** for rating prediction and **Recall@10, nDCG@10, and MAP@10** for recommendation generation, is provided in the report. Sensitivity analysis was also conducted to explore the impact of hyperparameters such as the number of neighbors (K) and latent factors.

## How to Run

1. Clone the repository:

   ```bash
   git clone https://github.com/yourusername/recommender-systems-project.git
    ```

2. Open the Jupyter notebooks to explore and run the experiments
