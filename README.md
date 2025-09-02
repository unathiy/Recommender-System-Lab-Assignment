# Recommender-System-Lab-Assignment

## Overview
This project implements a simple recommender system as part of the lab assignment.  
It demonstrates **Collaborative Filtering** and **Content-Based Filtering** using a small movie dataset.  

By the end of the lab, I:
- Understood the difference between Content-Based and Collaborative Filtering.
- Built a simple recommender system using Python and scikit-learn.
- Evaluated recommendations using cosine similarity.

---

## Dataset
The dataset is `movies_dataset.csv` and contains:
- `ID` → ID of the user  
- `MOVIE_TITLE` → Name of the movie  
- `RATING` → User’s rating (1–5)  
- `GENRE` → Movie genre(s), used for content-based filtering  

## Steps Implemented
### 1. Load the Dataset
Loaded the CSV file with pandas.

### 2. User-Item Matrix
Created a pivot table of users × movies with ratings.

### 3. Collaborative Filtering
Used cosine similarity on user-item matrix.
Recommended movies based on the most similar users.

### 4. Content-Based Filtering
Applied TF-IDF on movie genres.
Recommended movies similar to a chosen title (e.g., Toy Story).

### 5. Reflection
Compared both methods.
Discussed challenges (missing data, cold start, small dataset).
Suggested that a hybrid approach would work best.
