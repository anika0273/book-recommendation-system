# Book Recommendation System

## Overview

The Book Recommendation System aims to assist users in discovering new books based on their preferences. With the increasing number of online book retailers, an effective recommendation system is essential for enhancing user experience and increasing sales. This project focuses on building three types of recommendation systems:

1. **Knowledge/Rank Based Recommendation System**
2. **Similarity-Based Collaborative Filtering**
3. **Matrix Factorization Based Collaborative Filtering**

## Objective

To create a robust recommendation system that suggests books to users based on their interests and previous ratings. The project utilizes various algorithms to provide accurate recommendations, improving the shopping experience and increasing user engagement.

## Dataset

The project utilizes two datasets:

1. **Ratings Dataset**:
   - `user-Id`: Unique ID for each user
   - `ISBN`: International Standard Book Number identifying the book
   - `Book-rating`: Rating for each book on a scale from 0-10

2. **Books Dataset**:
   - `ISBN`: International Standard Book Number
   - `Book-title`: Title of the book
   - `Book-author`: Author of the book
   - `Year-of-Publication`: Publication year
   - `Publisher`: Publisher of the book
   - `Image-Url-S`: Small image of the book (Amazon link)
   - `Image-Url-M`: Medium size image of the book (Amazon link)
   - `Image-Url-L`: Large size image of the book (Amazon link)

## Algorithms

The following algorithms are implemented in this project:

1. **Rank-Based Recommendation**: 
   - Using averages to recommend books based on ratings.

2. **User-User Similarity-Based Collaborative Filtering**:
   - Identifying users with similar preferences and recommending books they have rated highly.

3. **Item-Item Similarity-Based Collaborative Filtering**:
   - Finding similarities between books and recommending items based on user interactions.

4. **Model-Based (Matrix Factorization) Collaborative Filtering**:
   - Decomposing the user-item matrix into lower-dimensional matrices to recommend books based on latent factors.

## Evaluation Metrics

Performance evaluation is done using the following metrics:

- **Precision@k**: Measures the accuracy of the top-k recommendations.
- **Recall@k**: Evaluates the ability to find relevant items among the recommendations.
- **F1 Score**: The harmonic mean of precision and recall, providing a balance between the two.

## Results

The optimized user-user similarity-based recommendation system achieved the best performance with an F1 Score of approximately **0.86**. The matrix factorization approach resulted in a lower RMSE of **1.50**, indicating its effectiveness in capturing latent factors that influence user preferences.

## Future Work

To further enhance the recommendation system, the following approaches can be considered:

- **Hyperparameter Tuning**: Fine-tuning model parameters to improve performance.
- **Hybrid Recommendation Systems**: Combining different recommendation techniques to create a more complex and accurate model.

## Getting Started

1. **Clone the Repository**:
   ```bash
   git clone <repository-url>
   cd Book-Recommendation-System
   ```

2. **Install Dependencies**:
   ```bash
   pip install -r requirements.txt
   ```

3. **Run the Project**:
   - Execute the main script to start the recommendation process.