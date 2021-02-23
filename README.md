# Overview
* You are given a stock dataset measured over a period of time. 
* A train set and a test set are given. 
* The goal is to learn about the train set and make predictions through the test set.

# Data Description
*Input data*
Each column of the data set consists of date information, item information, and feature set. The feature set is blurred. Features consist of data values ​​that are judged to be meaningful for each stock.

*Target data*
Two correct answer data for the train set are given, and the correct answer for the test set is given. The correct answer data is created with the following unit time (T) returns for each sample time.
Correct answer data 1: Unit time (T) Return (train_target.csv) -> Regression
Correct answer data 2: Target (train_target2.csv)-> Classification classified by dividing the unit time rate of return of the stocks (correct answer data 1) into 5 quartiles at a specific point in time.
