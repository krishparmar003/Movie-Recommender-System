# Movie Recommender System 🎬

A content-based movie recommender built from scratch. Give it a movie name and it finds 5 similar ones based on genre and plot — no ratings, no user history, just the content itself.

---

## How it works

Each movie gets a `tags` field combining its genre and plot overview. These tags are converted into vectors using TF-IDF, and cosine similarity is used to find the closest matches. Simple, fast, and works well for finding movies with a similar vibe.

```
Movie title → tags (genre + overview) → TF-IDF vectors → cosine similarity → top 5 recommendations
```

---

## Dataset

TMDB dataset with 10,000 movies. Each entry has title, genre, overview, popularity, release date, vote average, and vote count.

---

## Tech used

- **Pandas & NumPy** — data handling
- **Scikit-learn** — TF-IDF vectorization + cosine similarity

---

## Sample output

```python
recommend('Iron Man')

# Iron Man
# Mazinger Z: Infinity
# Justice League Dark
# Iron Man 3
# The Colony
```

---

## Run it locally

```bash
git clone https://github.com/krishparmar003/Movie-Recommender-System.git
cd Movie-Recommender-System
pip install -r requirements.txt
```

Open `movierecommender.ipynb` in Jupyter and run all cells.

---

## Structure

```
├── movierecommender.ipynb    # main notebook
├── dataset.csv               # TMDB movies dataset
├── requirements.txt
└── README.md
```
