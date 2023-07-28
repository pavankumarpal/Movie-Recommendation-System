# Movie-Recommendation-System
The movie recommendation system project aims to build a content-based movie recommender using Python. The system suggests movies to users based on their favorite movie, leveraging the genres and descriptions of movies to calculate similarity scores. The project includes the following steps:

1. Import Library: The necessary libraries are imported, including Pandas for data manipulation, NumPy for numerical computations, TfidfVectorizer for feature extraction, and cosine_similarity from scikit-learn for computing similarity scores.

2. Import Dataset: Load a movie dataset from external sources like CSV files or databases.

3. Get Feature Selection: The selected features used for similarity computation are 'Movie_Genre','Movie_Keywords','Movie_Tagline','Movie_Cast','Movie_Director' of the movies. These features will be combined to create a single string for each movie.

4. Get Feature Text Conversion to Tokens: The 'Movie_Genre','Movie_Keywords','Movie_Tagline','Movie_Cast'and 'Movie_Director' text data are combined to create a single text string for each movie. The text is then converted into tokens using the TfidfVectorizer. This process transforms the text into a numerical representation that can be used for similarity calculations.

5. Get Similarity Score using Cosine Similarity: Cosine similarity is a metric used to calculate the similarity between two non-zero vectors. In this case, it is applied to calculate the similarity between movies based on their feature tokens. The similarity scores are stored in a similarity matrix, where each cell represents the similarity score between two movies.

6. Get Movie Name as Input From User and Validate for Closest Spelling: The user is prompted to enter their favorite movie name as input. The program then validates the input by checking if the movie name exists in the dataset. If the movie name is misspelled or not found, the program suggests the closest match.

7. Get all Movies Sorted Based on Recommendation Score with respect to the Favorite Movie: Using the similarity matrix, the program retrieves the similarity scores between the user's favorite movie and all other movies in the dataset. The movies are then sorted based on their similarity scores, in descending order. The top recommended movies are selected based on this ranking.

8. Top 10 Movies Recommendation System: Finally, the program displays the top 10 movie recommendations to the user based on their favorite movie. These recommendations are made based on the similarity scores between the user's favorite movie and all other movies in the dataset.

 
