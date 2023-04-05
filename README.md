# MovieRecSys

## Overview

This dataset (ml-latest-small) describes 5-star rating and free-text tagging activity from [MovieLens](http://movielens.org), a movie recommendation service. It contains 100004 ratings and 1296 tag applications across 9125 movies. These data were created by 671 users between January 09, 1995 and October 16, 2016. This dataset was generated on October 17, 2016.

Users were selected at random for inclusion. All selected users had rated at least 20 movies. No demographic information is included. Each user is represented by an id, and no other information is provided.

This and other GroupLens data sets are publicly available for download at <http://grouplens.org/datasets/>.

## Performance Evaluation

We split the rating data into training and validation data at a 9:1 ratio. Using the training data, we predict the user's movie rating using the following three methods:

- Average rating for all movies
- Average rating for each user's movie
- Average rating for each movie

We calculate and compare the mean absolute error (MAE) and root mean squared error (RMSE) of the three methods to evaluate their performance.

## Exploiting Explicit Feedback

### Content-Based Filtering

We use item metadata to calculate similarity between items and represent a user's profile as a list of items with their respective ratings. We then recommend other items that are similar to the ones in the user's item list.

### Item-Based Collaborative Filtering

We calculate similarity between items using rating distribution and represent a user's profile as a list of items with their respective ratings. We then recommend other items that are similar to the ones in the user's item list.

### User Based Collaborative Filtering

We calculate similarity between users using rating distribution and estimate ratings based on the ratings given to each item by users similar to the target user.

## More Advanced Techniques

### Linear Regression

We create user profiles using a regression model and use these profiles to predict item ratings. We can also use regularization techniques to fine-tune the regression model.

### Matrix Factorization

We abstract users and items using singular value decomposition (SVD) and calculate similarity between abstracted items.
