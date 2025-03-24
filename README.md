# Movie Recommendation System using Machine Learning

A content-based movie recommendation system with both Jupyter notebook analysis and a Streamlit web interface that suggests similar movies based on their features.

## Features
- **Web Interface**: Interactive UI built with Streamlit
- **Recommendation Engine**: Suggests 5 most similar movies for any given movie title
- **Content-Based**: Uses movie features like genres, keywords, cast, and crew
- **Data Processing**: Cleans and combines multiple features for accurate recommendations

## Technologies Used
- Python
- Streamlit (for web interface)
- Pandas (for data manipulation)
- Scikit-learn (for CountVectorizer and cosine similarity)
- Numpy
- Ast (for literal evaluation of strings)

## Dataset
The system uses the [TMDB 5000 Movies Dataset](https://www.kaggle.com/datasets/tmdb/tmdb-movie-metadata) which contains:
- 4806 movies
- Features like genres, keywords, cast, crew, overview, etc.

## How It Works
1. **Data Processing**:
   - Data is loaded and merged from two CSV files
   - Features are processed and combined into tags
   - Text data is vectorized using CountVectorizer
   - Cosine similarity is calculated between all movies

2. **Web Interface**:
   - User selects a movie from dropdown
   - System displays movie poster and details
   - Shows 5 most similar movies with their posters

## Installation
1. Clone the repository
2. Install required packages:
   ```bash
   pip install pandas scikit-learn numpy streamlit
