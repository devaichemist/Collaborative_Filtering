# Collaborative Filtering Recommender Systems

This notebook presents the development of a collaborative filtering recommender system for predicting movie preferences. It uses a reduced subset of the MovieLens dataset, which includes thousands of user-movie ratings. The model captures patterns by representing users and movies as vectors within a shared feature space, where predicted ratings are computed through vector interactions and user-specific bias terms.

The collaborative filtering cost function is implemented from scratch, with regularization included to improve generalization and prevent overfitting. Both loop-based and vectorized versions of the function are provided to balance clarity and performance. Training is done through a custom loop built with TensorFlow’s GradientTape, allowing direct control over the optimization process and efficient parameter updates.

Once trained, the model can accept user-defined movie ratings to generate personalized predictions for unseen titles. The output is refined using Pandas filtering techniques, allowing recommendations to be sorted and interpreted based on average ratings and popularity metrics.

## Results

The collaborative filtering model successfully learned user preferences and movie features.

The training loss decreased significantly over 200 iterations, indicating successful learning:

Initial loss: 2,321,191.3

Final loss: ~2,902.1

Personalized recommendations were generated for a new user based on their selected movie ratings. High-confidence predicted ratings include:

4.49 for My Sassy Girl (2001)

The model also accurately predicted the user’s known ratings:

Shrek (2001) — Original: 5.0, Predicted: 4.90
