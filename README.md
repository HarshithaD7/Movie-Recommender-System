# Movie Recommender System

## Project Description
This project implements a **content-based movie recommender system** that suggests movies similar to a given movie based on **metadata similarity**.  
The system is built and executed entirely in a **Kaggle Notebook environment**.

Instead of predicting ratings, the model computes **similarity between movies** using textual features such as genres, keywords, cast, crew, and overview.

---

## Objectives
- Load and preprocess movie metadata
- Combine multiple textual attributes into a single feature space
- Convert text data into numerical vectors
- Compute similarity between movies
- Recommend top-N similar movies for a given input title

---

## Dataset
- Movie metadata dataset containing:
  - Title
  - Genres
  - Keywords
  - Cast
  - Crew
  - Overview
- Each row represents a single movie

> Due to size limitations, only sample files are included in the repository.  
> The full dataset is processed inside the Kaggle notebook.

---

## Approach Used
- Feature combination (genres + keywords + cast + crew + overview)
- Text vectorization using **CountVectorizer**
- Similarity computation using **Cosine Similarity**
- Ranking movies based on similarity scores

---

## Results Overview
- The system successfully recommends movies with similar themes, genres, and cast
- Recommendations are deterministic and explainable
- No user-rating data is required

Detailed evaluation and analysis are available in:
- `results/metrics.md`
- `results/observations.md`

---

## Source Code
- Complete implementation is provided in the `src/` folder as a Jupyter Notebook.

---
