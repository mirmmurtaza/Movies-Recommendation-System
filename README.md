# Movies Recommendation System

This project aims to develop a movie recommendation system that suggests five movies similar to a given movie assuming that the user previously watched the given movie. The recommendation system is built using the IMDB movie dataset, which contains relevant columns such as title, genre, imdb rating, and overview. The genre column is categorical, whereas the overview column is textual and contains descriptions of the movies.

To build the recommendation system, the categorical genre column was converted into a numerical representation using CountVectorizer. The overview column was converted into sentence embeddings using DistilBERT-base-nli-mean-tokens. Once the data was transformed into an appropriate representation, cosine similarity was used to compute the similarity matrix.

Using the similarity matrix, the recommendation system suggests five movies that are similar to the movie the user watched previously.
