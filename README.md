# Board Game Review Prediction

* In this project, we have a dataset containing 80,000 board games and their corresponding review scores. These data was scraped from BoardGameGeek. The data contains rows and columns, Each row represnets a single board game and has statiistics about the board game as well as review information.
* The aim of this project is to predict average_rating using the other columns. Since the dataset contained a few missing values and there were rows without reviews, where there is a score of 0, it was removed.
## PreProcessing the dataset
* The columns [‘id’, ‘type’, ‘name’, ‘bayes_average_rating’] are to be dropped.
* The rows with missing values are to be dropped.
* The rows with ‘users_rated’ = 0 are to be dropped.

## Training the model
* The data set has been preprocessed and is ready to be trained. A comparison is made between 2 models :- Linear Regression & Random Forest Regression.

## Result
* After using Linear Regression model, I found out that the Mean Squared Error(MSE)=2.078 which is greater than 0, making a Linear model unfit for this prediction, hence we tried the Random Forest Regressor, which was eventually generating prediction value close to the actual values by a tiny fraction.
* As expected the performance of Random Forest Regressor model is better than Linear Regression model for the given data set. This is because the board game data set is very large and it is difficult for the Linear Regression model to fit the data by a straight line.
