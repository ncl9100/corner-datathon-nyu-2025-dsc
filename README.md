# Corner App - Challenge 1 - User Taste Clustering Datathon (NYU DSC Datathon 2025)

## Project Overview

This project explores clustering users based on their place visit histories from two cities (New York and San Francisco).

## Objectives

- Cluster users based on the places they have visited.
- Identify pivot places that define user taste clusters.
- Analyze city-based behavior differences.
- Handle cold start challenges (users with few interactions).

## Dataset

- **places.csv** – Place metadata (tags, description, embedding, etc.)
- **user_place.csv** – User interactions (visited / favorited)
- **users.csv** – User IDs

## Dataset Access

📁 **Note:**  
The full datasets (`places.csv`, `user_place.csv`, `users.csv`) are excluded from this repository due to GitHub's file size limitations (files larger than 100MB).  
If you'd like access to a sample dataset or the full dataset for testing purposes, please contact Corner.

## Methods

- Clean and process embeddings.
- Average embeddings per user.
- Project high-dimensional embeddings into 2D using t-SNE.
- Cluster users using HDBSCAN (density-based clustering).
- Analyze pivot places, city distributions, and common tags.
- Handle cold start users separately.

## Key Findings

- Distinct taste clusters based around specific types of places (e.g., cozy restaurants, hidden bars).
- City (New York vs San Francisco) was moderately predictive of clustering.
- Pivot places act as strong indicators of user similarity.
- Cold start users require special handling due to sparse data.

## Tools Used

- Python (Pandas, scikit-learn, HDBSCAN, t-SNE, Matplotlib)
- Jupyter Notebook
- Excel (for final pivot place analysis)

## Author

Nathan Liu  
`corner-datathon-nyu-2025`
