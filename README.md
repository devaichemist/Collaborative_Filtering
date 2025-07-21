# Collaborative Filtering Recommender Systems

In this notebook we'll build a movie recommendation system using collaborative filtering. Specifically, it involves implementing and optimizing a collaborative filtering cost function to learn feature vectors for movies and preference parameters for users based on historical movie ratings. The model predicts a user's potential rating for an unrated movie based on learned user and item vectors and their biases. The collaborative filtering algorithm should minimize the cost function representing the error between actual and predicted ratings, including regularization to prevent overfitting.

## Results

The collaborative filtering model successfully learned user preferences and movie features.

The training loss decreased significantly over 200 iterations, indicating successful learning:

Initial loss: 2,321,191.3

Final loss: ~2,902.1

Personalized recommendations were generated for a new user based on their selected movie ratings. High-confidence predicted ratings include:

4.49 for My Sassy Girl (2001)

The model also accurately predicted the user’s known ratings:

Shrek (2001) — Original: 5.0, Predicted: 4.90
