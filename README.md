 Movie Recommendation System

This is a content-based movie recommendation system built using Python, Streamlit, and machine learning techniques. The system suggests movies that are similar to a selected title by analyzing the content features such as genres, overview, cast, and keywords. It uses cosine similarity to identify and recommend top similar movies and fetches movie posters using The Movie Database (TMDB) API. The application provides an interactive web interface for users to explore recommendations quickly and easily.

## Features

- Movie selection from an interactive dropdown
- Content-based recommendations using similarity scores
- Automatic fetching of movie posters via TMDB API
- Clean and simple user interface using Streamlit

### Large Model File

Due to GitHub file size limits, the `.pkl` model is hosted externally.

📦 [Download similarity.pkl from Google Drive](https://drive.google.com/file/d/16SgdckApXvAds8xQj9YKj-ZAI7WDY1V9/view?usp=drive_link)


## Project Structure

movie-recommender-system/
│
├── app.py # Streamlit application file
├── movie-recommender-system.ipynb # Jupyter notebook for preprocessing
├── movies_dict.pkl # Pickle file storing movie metadata
├── similarity.pkl # Pickle file storing similarity scores
├── tmdb_5000_movies.csv # Source dataset
├── requirements.txt # Python dependencies
├── README.md # Project documentation

## Installation and Setup

1. Clone the repository:

git clone https://github.com/yourusername/movie-recommender-system.git
cd movie-recommender-system

markdown
Copy
Edit

2. Install the required Python packages:

pip install -r requirements.txt

markdown
Copy
Edit

3. Run the Streamlit application:

streamlit run app.py

The application will open in your default web browser at `http://localhost:8501`.

## TMDB API Key

This project uses the TMDB API to fetch movie posters. Make sure to use a valid API key. The key is hardcoded in `app.py`. If needed, generate a new API key from https://www.themoviedb.org/settings/api and replace the existing key in the code.

## Requirements

The required Python libraries are listed below:

streamlit==1.35.0
pandas==2.2.2
scikit-learn==1.4.2
numpy==1.26.4
requests==2.31.0

You can install them using:

pip install -r requirements.txt

## How It Works

- Movie metadata is processed and transformed into a feature vector.
- Cosine similarity is computed between all movie vectors.
- When a user selects a movie, the system finds and returns the most similar titles based on the similarity matrix.
- Posters for the recommended movies are fetched from TMDB using their API.

## Author

This project was developed by Bhanu Deergasi. You can reach out through your GitHub profile at https://github.com/bhanudeergasi

## License

This project is licensed under the MIT License. You are free to use, modify, and distribute this project for personal or commercial purposes.
