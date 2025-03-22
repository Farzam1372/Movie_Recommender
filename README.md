# 🎬 Movie Recommender System

This project implements a **Hybrid Movie Recommender System** using both **Content-Based Filtering** and **Collaborative Filtering**. Built with **pure Python, NumPy, and Scikit-Learn**, and deployed with **Streamlit**, this app suggests movies tailored to a user's preferences.

## 💡 Features

- ✅ Content-Based Filtering using TF-IDF and Cosine Similarity
- ✅ Collaborative Filtering using Singular Value Decomposition (SVD)
- ✅ Hybrid approach combining both methods
- ✅ Interactive Web App with Streamlit
- ✅ Pure Python implementation (no high-level libraries like `surprise`)
- ✅ Reproducible pipeline from data to deployment

---

## 📁 Dataset

- **Source**: [MovieLens 100K (ml-latest-small)](https://grouplens.org/datasets/movielens/)
- Contains:
  - 100,000+ ratings from 600 users on 9,000+ movies
  - Metadata: Titles, Genres, Tags, IMDb & TMDB links

---

## 🚀 How It Works

### 📊 1. Data Processing
- Load `ratings.csv`, `movies.csv`, and `tags.csv`
- Merge data for unified access
- One-hot encode genres
- Apply TF-IDF on movie titles or tags

### 🧠 2. Model Building

#### Content-Based Filtering
- TF-IDF vectors → Cosine similarity
- Recommend similar movies based on content

#### Collaborative Filtering
- Build user-item rating matrix
- Apply SVD with NumPy to learn latent features
- Predict unseen user ratings

#### Hybrid Model
- Combine both systems via weighted average
- Tunable `alpha` parameter controls influence of each model

### 🌐 3. Web App (in Progress)
- Built using Streamlit
- Allows user selection, model tuning, and recommendation display

---
