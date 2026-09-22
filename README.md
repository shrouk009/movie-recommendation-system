# 🎬 Movie Recommendation System

## 📌 Project Overview

This project implements a movie recommendation system using the
MovieLens 100K dataset.

The system uses collaborative filtering techniques to recommend
movies based on similarities between users and their rating patterns.

The project explores both user-based and item-based collaborative
filtering, as well as matrix factorization using SVD.

---

## 📊 Dataset

The project uses the MovieLens 100K dataset.

The dataset contains approximately:

- 100,000 movie ratings
- 943 users
- 1,682 movies
- Ratings from 1 to 5

Main files used:

- `u.data` — user ratings
- `u.item` — movie information and titles

---

## 🛠 Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn
- Google Colab

---

## 🔍 Project Workflow

### 1. Data Loading and Exploration

The MovieLens rating data was loaded and explored to understand:

- Number of users
- Number of movies
- Number of ratings
- Rating distribution

### 2. User-Item Matrix

A user-item matrix was created where:

- Rows represent users
- Columns represent movies
- Values represent movie ratings

Missing ratings represent movies that a user has not rated.

### 3. User-Based Collaborative Filtering

Cosine similarity was used to calculate similarity between users.

The system identifies users with similar rating patterns and uses
their preferences to recommend unseen movies to a target user.

### 4. Weighted Recommendations

Recommendations were improved by weighting ratings according to
user similarity.

Users with higher similarity have a greater influence on predicted
movie ratings.

### 5. Movie Recommendations

The system recommends the highest-rated unseen movies and displays
their movie titles and predicted ratings.

### 6. Evaluation

The recommendation system was evaluated using Precision@K.

Precision@K measures the proportion of recommended movies that are
relevant to the user among the top K recommendations.

### 7. Item-Based Collaborative Filtering

As an additional experiment, item-based collaborative filtering was
implemented.

Instead of finding similar users, this approach calculates similarity
between movies based on user rating patterns.

### 8. Matrix Factorization

Truncated SVD was explored to reduce the user-item matrix into
latent features.

This provides an introduction to matrix-factorization-based
recommendation systems.

---

## 🧠 Recommendation Approach

The main recommendation pipeline is:

User Ratings
→ User-Item Matrix
→ Cosine Similarity
→ Similar Users
→ Weighted Ratings
→ Remove Already Rated Movies
→ Top Movie Recommendations

---

## 📈 Evaluation Metric

The primary evaluation metric used in this project is:

**Precision@K**

It evaluates how many of the top K recommended movies are relevant
to the user.

---

## 💡 Key Takeaways

- Collaborative filtering can generate recommendations without
  requiring movie genre information.
- Cosine similarity can identify users with similar preferences.
- Similarity-weighted ratings can improve recommendation ranking.
- Item-based filtering provides an alternative to user-based filtering.
- Precision@K can be used to evaluate recommendation relevance.
- Matrix factorization can represent users and movies using latent factors.

---

## 🚀 Future Improvements

Possible improvements include:

- More rigorous train/test evaluation
- Recall@K and F1@K
- Hyperparameter tuning
- Improved SVD-based recommendations
- Hybrid recommendation systems
- Incorporating movie genres and metadata

---

## 👤 Author

Shrouk Ahmed

Machine Learning Portfolio Project
