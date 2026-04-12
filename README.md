# Movie Recommendation System 🎬

**[🔴 View Live Application](https://movie-recommend-ajinkyasatuse.streamlit.app/)**

A machine learning-powered web application that suggests highly relevant films based on user interests. By analyzing extensive movie metadata—including genres, keywords, cast, and crew—this content-based filtering system identifies the "hidden" connections between films to deliver personalized recommendations. 

## 🚀 Core Features
* **Smart Search:** Instantly find recommendations tailored to your tastes from a curated dataset of over 5,000 popular movies.
* **Content-Based Filtering:** Leverages Natural Language Processing (NLP) to recommend movies based on thematic and structural similarities rather than just user ratings.
* **Dynamic Visuals:** Integrates with the TMDB API to fetch and display high-quality, real-time movie posters for an immersive and visual user interface.
* **Interactive Interface:** A responsive, lightweight, and user-friendly frontend powered by Streamlit.

## 🧠 How It Works (The Pipeline)
The recommendation engine processes data through a strict three-step pipeline:

1. **Data Preprocessing:** We aggregated raw metadata (genres, overviews, cast, and crew) from the TMDB 5,000 dataset into a unified `tags` column. We then applied **Stemming** (via NLTK) to normalize the text and reduce words to their root forms.
2. **Text Vectorization:** Using Scikit-Learn’s `CountVectorizer`, the processed text data was transformed into a 5,000-dimensional vector space, turning qualitative movie data into quantitative mathematical data.
3. **Similarity Calculation:** To determine how closely related two movies are, the system calculates the **Cosine Similarity** between their vectors. By measuring the cosine of the angle between vectors (rather than Euclidean distance), the system accurately pairs movies with the highest thematic overlap.

## 🛠️ Tech Stack
* **Language:** Python
* **Machine Learning:** Scikit-Learn, NLTK (Natural Language Toolkit)
* **Data Manipulation:** Pandas, NumPy
* **Frontend/Framework:** Streamlit
* **External Services:** TMDB API (The Movie Database) for poster generation
