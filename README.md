Song Recommendation System 🎵

A content-based music recommendation system built using Python, Flask, and key libraries like Pandas, Scikit-learn, and Pickle. The system analyzes song metadata and provides personalized recommendations based on user input.

# Features

  •	Recommends songs similar to a user-input song using content-based filtering.
	•	Interactive web interface for entering song titles and retrieving recommendations.
	•	API for retrieving all available songs and fetching recommendations programmatically.
	•	Efficient cosine similarity algorithm for calculating song similarity.



# Installation

## Prerequisites

	•	Python 3.7+
	•	Flask
	•	Pandas
	•	Scikit-learn

## Setup

1. Clone this repository:
   ```bash
   git clone https://github.com/Saahilarious/Song_Recommendation_system
   cd Song_Recommendation_system


       

2.	Install required dependencies:

 	•	Flask (for the web application framework)
	•	Pandas (for data processing and manipulation)
	•	Scikit-learn (for similarity calculations and vectorization)
	•	Pickle (for saving and loading the model; comes built-in with Python)


3.	Run the application:
    ```bash
  	 python app.py  

 4.	Open your browser and navigate to http://127.0.0.1:5000.

# Dataset

The system uses a Spotify dataset containing features like song titles, artists, genres, and user ratings. The data was cleaned, preprocessed, and enriched with additional features for better recommendations.

# Workflow

## Data Preparation

  1.	Load and clean the dataset (handle missing values, duplicates, and normalization).
	2.	Combine relevant features (artist, genre, album, etc.) into a single “tags” column.
	3.	Vectorize the tags using CountVectorizer to prepare for similarity calculations.

## Recommendation Logic

  •	Use cosine similarity to measure the closeness between songs based on their tags.
	•	Create a similarity matrix to store scores between all song pairs.
	•	Fetch the top recommendations for a given song.

## Web Application

  •	Built with Flask for simplicity and scalability.
	•	Routes:
	•	/: Home page for user input.
	•	/recommend: API endpoint for fetching recommendations.
	•	/songs: API endpoint for retrieving all available songs.

# Example Usage

  1.	Enter a song title in the web app or send a request to /recommend.
	2.	The system returns a list of songs similar to the input.

# Future Enhancements

  •	Integrate collaborative filtering for user-specific recommendations.
	•	Add audio feature analysis (tempo, rhythm, etc.) for deeper insights.
	•	Include real-time data updates and integration with music streaming APIs.

# Technologies Used

  •	Backend: Flask
	•	Data Processing: Pandas, Scikit-learn
	•	Similarity Calculation: Cosine Similarity
	•	Serialization: Pickle

# Contributions

Feel free to open issues and contribute via pull requests!
