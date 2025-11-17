Movie Recommendation System with Cosine Similarity
Overview
This project builds a simple movie recommendation system using the MovieLens dataset. It combines movie ratings, user tags, and metadata to create a richer representation of movies. By applying TF-IDF vectorization and cosine similarity, the system suggests movies that are most similar to a given title.
Dataset
•	Source: MovieLens small dataset
•	Files used: movies.csv, ratings.csv, tags.csv, links.csv
•	Data merged on movieId for complete user/movie records
Methods
•	Data cleaning and merging using pandas
•	Pivot tables for user-movie matrices
•	TF-IDF for text features (tags)
•	Cosine similarity to measure closeness between movies
•	Recommendation function to return the top N most similar movies
Results
When a user enters a movie title, the system returns a list of recommended films. Testing with "Homeward Bound: The Incredible Journey (1993)" produced relevant family-friendly and adventure-themed movie suggestions.
Tools
•	Python (pandas, scikit-learn)
•	Jupyter Notebook
Future Work
•	Add genre and cast information for deeper recommendations
•	Include collaborative filtering techniques
•	Build a user interface for easier interaction

