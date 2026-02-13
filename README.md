# 🎬 Movie Recommendation System

A content-based movie recommendation system that suggests similar movies based on a user-selected title.  
This project uses **TF-IDF vectorization** of movie metadata (overview, genres, keywords, cast, director) and computes **pairwise similarity** using kernels such as cosine similarity or sigmoid kernel.

---

## 🔹 Features
- Content-based filtering: recommends movies similar to the chosen title.
- TF-IDF vectorization of movie metadata.
- Pairwise similarity computation using cosine or sigmoid kernel.
- Returns top 10 most similar movies.
- Easy to extend with APIs (e.g., TMDb for posters/details).
- Scalable for deployment with Flask, FastAPI, or Streamlit.

---

## 🔹 Tech Stack
- **Python 3.x**
- **Pandas** for data handling
- **Scikit-learn** for TF-IDF and similarity kernels
- **NumPy** for numerical operations
- **Streamlit/Flask** (optional) for UI

---

## 🔹 Workflow
1. Load and clean movie dataset (`movies_cleaned_df`).
2. Build TF-IDF matrix from textual features.
3. Compute similarity matrix using chosen kernel.
4. For a given movie title, sort similarity scores.
5. Return top 10 most similar movies.

---

## 🔹 Example Usage
```python
# Example: Get recommendations for Avatar
recommendations = give_recommendations("Avatar")
print(recommendations)
