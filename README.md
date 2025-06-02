# Recommender System Homework Repository

## Overview
This repository hosts the complete solution for a detailed Recommender System homework assignment. The project encompasses a wide range of topics in recommender systems, implemented and analyzed using Python. It includes data processing, similarity computations, collaborative filtering, latent factor modeling, and performance evaluations, all documented in a single Jupyter notebook.

## Project Structure
- `Recommender System HW.ipynb`: The main Jupyter notebook containing all code, analyses, and discussions.
- `/home/wajason99/datamininghw5/hw5 data/ratings.train.txt`: Training data file (ensure this is included or referenced appropriately).
- `shows.txt`: File containing show names (ensure this is included or referenced).
- `README.md`: This file, providing an overview and instructions.

## Contents
### Section 1: Similarity Computations
- **Task 1.a**: Computation of Jaccard Similarity between users based on binary watch data.
- Detailed manual calculations and verification using `sklearn.metrics.jaccard_score`.
- Identified the most similar user pairs (e.g., Willy & Xavier with a similarity of 0.75).

### Section 2: Collaborative Filtering
- Implementation of **User-User** and **Item-Item** collaborative filtering on a real dataset with 9985 users and 563 shows.
- Processed `user-shows.txt` and `shows.txt` to generate recommendation lists for user "Jim" (index 499).
- Recommendations include top 5 shows with scores, ensuring handling of ties by prioritizing lower indices.

### Section 3: Latent Factor Recommendation
- Developed a matrix factorization model using Stochastic Gradient Descent (SGD).
- Tuned learning rates (e.g., 0.1 to 0.00001) with 40 iterations, analyzing convergence curves.
- Explored a refined range [0.008, 0.015] with additional points (e.g., 0.0117) to minimize total error (best E = 48490.77).
- Visualizations compare all learning rates and a subset [0.05, 0.02, 0.01, 0.001] plus the best external rate.

## Mathematical Derivations
- Proof of the item-item similarity matrix \( S_I = Q^{-1/2} R^T R Q^{-1/2} \).
- Derivation of the user-user similarity matrix \( S_U = P^{-1/2} R R^T P^{-1/2} \).
- Discussions on convergence behavior, learning rate impacts, and regularization effects.

## Run the Notebook:
Open Recommender System HW.ipynb in Jupyter Notebook or JupyterLab and execute the cells.
