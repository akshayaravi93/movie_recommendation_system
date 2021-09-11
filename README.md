# movie_recommendation_system

## Collaborative filtering: 

### Movie Recommendation by prediction of customer rating for a movie

Goal : Finding customer rating for movies using truncated SVD.

Here basic python libraries like numpy, pandas and scipy are only used to understand the algorithm better.

- Consider we have input information of customer rating given by different users for different movies.
- We can predict the customer rating of a user for a movie that he /she has not rated yet and thereby recommend them new movies.
- Since input information (utility matrix) is a sparse matrix, SVD can be used to decompose the user-movie interaction. Here features are selected based on the RMSE function. 
- For the feature 12, it was found that the RMSE value is minimum and hence SVD with features 12 has been used.

Inspired from Netflix competition, https://towardsdatascience.com/the-netflix-prize-how-even-ai-leaders-can-trip-up-5c1f38e95c9f

Credits to
https://towardsdatascience.com/beginners-guide-to-creating-an-svd-recommender-system-1fd7326d1f65 for the reference on the code. Code was adapted to match the latest python version and for additional visualisations.
https://towardsdatascience.com/movie-recommendation-system-based-on-movielens-ef0df580cd0e for the reference on the dataset

## Content based method: 

### Movie content based recommendation using similarity measures

Goal: Recommend movies based on the closeness (distance) between two movies

- In case of cold start problem for recommendation systems, there is possibility that the new user has not rated the movie yet.
- One remedy is, This new user would have filled user data (they might have filled if they like comedy, or certain movie or so)
- If we can find how close the two movies are and relate it to the user data, new top 10 movie can be recommended for that user

Credits to https://www.geeksforgeeks.org/movie-recommender-based-on-plot-summary-using-tf-idf-vectorization-and-cosine-similarity/ for the code reference. Here the code is adapted to our scenario, checked with respect to movie description and genres
