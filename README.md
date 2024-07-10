# Movie Recommendation System

This project implements a content-based movie recommendation system using machine learning techniques.

## Technologies Used

- Python
- Pandas
- Scikit-learn
- Streamlit
- TMDB API

## How It Works

1. **Data Preprocessing**: 
   - Movie data is cleaned and processed from TMDB dataset.
   - Features like genres, keywords, cast, and crew are extracted and combined.

2. **Feature Extraction**:
   - Text data is converted into numerical vectors using CountVectorizer.

3. **Similarity Calculation**:
   - Cosine similarity is computed between movie vectors to measure their similarity.

4. **Recommendation Engine**:
   - When a user selects a movie, the system finds the most similar movies based on cosine similarity scores.
   - Top 5 similar movies are recommended.

5. **User Interface**:
   - Streamlit is used to create a web interface where users can select a movie and get recommendations.
   - Movie posters are fetched from TMDB API for visual representation.

## How Similarity is Decided

The similarity between movies is determined using cosine similarity on the feature vectors. This method compares the angle between vectors in a multi-dimensional space, where each dimension represents a unique word or feature. Movies with more common features will have a higher similarity score.
