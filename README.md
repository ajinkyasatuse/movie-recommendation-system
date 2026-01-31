Live Link : https://movie-recommend-ajinkyasatuse.streamlit.app/

A Content-Based Movie Recommendation System built with Python and Scikit-Learn. Leveraging Cosine Similarity on the TMDB 5,000 dataset to suggest films based on metadata. Features real-time poster fetching via TMDB API.
It is a machine learning-powered web application that suggests movies based on the user's interests. By analyzing movie metadata like genres, keywords, cast, and crew, the system identifies similarities between films to provide highly relevant recommendations.
🚀 Features
Smart Search: Find recommendations for over 5,000 popular movies from the TMDB dataset.
Content-Based Filtering: Uses NLP and vectorization to find "hidden" connections between movies.
Dynamic Visuals: Fetches real-time movie posters using the TMDB API for an immersive UI.
Interactive Interface: (Mention your framework here, e.g., Streamlit, Flask, or React).
🧠 How It Works
The recommendation engine follows a three-step pipeline:
Data Preprocessing: We combined movie tags (genres, overview, cast, and crew) into a single "tags" column and applied Stemming to normalize the text.
Vectorization: Using Scikit-Learn’s CountVectorizer, we converted the text data into a 5,000-dimensional vector space.
Similarity Calculation: Instead of Euclidean distance, we used Cosine Similarity to calculate the distance between vectors. The closer the cosine angle, the more similar the movies.
