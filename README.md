# Machine_Learning_Team7
Beer recommendation system

## Dataset
* https://www.kaggle.com/datasets/rdoume/beerreviews

### Function

1. sort_best_beer_order
   * sort dataSet by recommend list from parameter
   * param data: entire dataSet
   * param recommend_list: list of best beers to recommend
   * return: dataSet sorted by recommend list
2. get_user_profile
   * get preference information by user's beer style based on review rating
   * param user_info: dataFrame for existing review data from user
   * param ohe: one-hot-encoded dataFrame for "beer style" on entire dataSet
   * return: normalized weight rating matrix of beer style of a user
3. recommend_content_based
   * recommend beers using content-based recommendation system based on a user's history
   * param data: entire dataSet
   * param user_name: a string for user name from review data
   * param num_c: number of beer styles to recommend
   * param num_b: number of beers per beer style to recommend
   * return: final recommended beer name with beer style and brewery name
4. predict_rating
   * predict rate
5. get_mse
   * evaluation MSE only for the beers rated by the user
6. get_rmse
   * create prediction R matrix
   * extract the RMSE of the actual R matrix and the predicted matrix by extracting the position index of non-null values from the actual R matrix
7. matrix_factorization
   * matrix factorization function
8. recommend_item_based_neighbor
