# MovieRecSys

## Summary

This dataset (ml-latest-small) describes 5-star rating and free-text tagging activity from [MovieLens](http://movielens.org), a movie recommendation service. It contains 100004 ratings and 1296 tag applications across 9125 movies. These data were created by 671 users between January 09, 1995 and October 16, 2016. This dataset was generated on October 17, 2016.

Users were selected at random for inclusion. All selected users had rated at least 20 movies. No demographic information is included. Each user is represented by an id, and no other information is provided.

This and other GroupLens data sets are publicly available for download at <http://grouplens.org/datasets/>.

## Performance Evaluation

Practice calculating MAE and RMSE based on Movielens rating data. The rating data is split 9:1 into training and validation data. Using the training data, we predict the user's movie rating using the following three methods.

- Average rating for all movies
- Average rating for each user's movie
- Average rating for each movie

Calculate and compare the MAE and RMSE of the three methods.

## Exploiting Explicit Feedback

### Content Based Filtering

- Calculate similarity between items using item metadata
- Represent a user profile as a list of items with user ratings
- Create other items that are similar to items in the item list as recommended items

### Item Based Collaborative Filtering

- Calculate similarity between items using rating distribution
- Represent a user profile as a list of items with user ratings
- Create other items that are similar to items in the item list as recommended items

### User Based Collaborative Filtering

- Calculate similarity between users using rating distribution
- Estimating ratings based on ratings given to each item by users similar to you
