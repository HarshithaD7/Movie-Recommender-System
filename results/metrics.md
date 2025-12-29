# Evaluation Metrics  
## Movie Recommender System

This project implements a **content-based recommender system**, which is evaluated differently from regression or classification models.

---

## Similarity Metric Used

### Cosine Similarity
- Measures similarity between movie feature vectors
- Computed on CountVectorizer-generated vectors
- Higher cosine similarity indicates stronger content similarity

---

## Feature Representation
- Textual attributes combined into a single feature string:
  - Genres
  - Keywords
  - Cast
  - Crew
  - Overview
- Vectorization method: **CountVectorizer**
- Stop words removed during vectorization

---

## Recommendation Logic
- A cosine similarity matrix is computed for all movies
- For a given movie title:
  - Similarity scores are retrieved
  - Movies are sorted in descending similarity order
  - Top-N most similar movies are returned

---

## Notes on Evaluation
- No numerical accuracy (MAE, RMSE, etc.) is used
- Evaluation is based on:
  - Relevance of recommendations
  - Consistency of similarity ranking
  - Semantic similarity between recommended movies
