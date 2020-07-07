# CKME-136-Movie-recommender: Methodology to execute the Initial code and Result.

## 1 Used Libraries
**Line 16** - In this Data Science project, the following packages were  used – ‘recommenderlab’, ‘dplyr’,  ‘ggplot2’, ‘data.table’ and ‘reshape2’ was executed.

## 2 Loading Dataset into R
**Line  33** - The following datasets were executed next to load into a data frame in R
•	Movies dataset – IMDb_movies.csv
•	Ratings dataset – IMDb_ratings.csv
**Line  40** - Loads a summary of movies and ratings dataframes in R together with the first several first rows.

## 3 DATA PREPROCESING STEP
###### 3.1 Extract a list of genres 
**Line  53** – Loads a matrix that reorganizes movie genre information for each of the films”. This will allow future users search for movies they like within a specific genre.
###### 3.2	Search Matrix
**Line  88** – Load this to allow us to perform an easy search of the films by specifying its genre present in the list.
###### 3.3	Converting ratings matrix in a proper format
**Line  94** - Load this in order to use ratings data for building a recommendation engine with “recommenderlab” library package by creating a matrix of users and films and ratings of all films by each user.

## 4	Exploring Parameters of Recommendation Models and Similarity Data between Users and Movies.
**Line  104** - Next step is to load the options for recommender model.
###### 4.1	Exploring Similarity Data – Users
**Line  115** - With the help of “recommenderlab”, we can compute similarities between the first four users using various methods like cosine, pearson and jaccard and then visualize it as an image.
###### 4.2	Exploring Similarity Data – Films
**Line  123** - With the help of “recommenderlab”, we can compute similarities between the first four films using various methods like cosine, pearson and jaccard and then visualize it as an image.

## 5	Further data exploration
**Line  130** – Load to display the different ratings and frequency their values as a table in the ratings dataframe, “IMDb_ratings.csv”.
###### 5.1	Distribution of ratings in the data frame.
**Line  139** - According to the documentation, a rating equal to 0 represents a missing value, so it was removed from the dataset before visualizing the results.

## 6	Movies Visualization
###### 6.1	Number of views of the top movies
**Line  149** & **Line  165** – Load to display section displays what the most viewed movies are and a bar plot of the total count of the top 6 viewed films.
6.2	Heatmap of Movie Ratings
**Line  175** -Load this section is executed to display the “whole matrix of ratings” and “first 20 rows and columns” where each row represents users ,columns represents movies and color shade intensity represents ratings

## 7	DATA PREPARATION (Movie Ratings)
###### 7.1	Selecting Useful Data
**Line  187** -Load this to reduce the number of users and movies in the dataset based on a threshold of number of films rated and number of users who have rated a film.
###### 7.1.1	Heat Map of top users and movies in the Movie rating threshold 
**Line  196** -Load this section selects the most relevant data based on the top 2 percent of users and movies in the new matrix of the most relevant data.
###### 7.1.2	The distribution of the average ratings per user in the ratings “IMDb_ratings” dataset.
**Line  204** –Load to view the Histogram plot of the average rating per user in the ratings dataframe.
###### 7.2	Normalization
**Line  212** – Load to view the Normalized dataset aimed at removing bias of high or low ratings provided to all films by a user.
###### 7.3	Data Binarization and Heatmap of the top users and movies
**Line  221** – Implemented make the classifier algorithm more efficient. By creating a rating threshold “0 – 3” as 0 and “3 – 5” as 1 : Define a matrix equal to 1 if the movie has been watched.

## 8	Defining Training and Test sets.
**Line  231** – Displays and splits the training and test dataset parameters. 

## 9	ITEM-based Collaborative Filtering Model Implementation
###### 9.1	Displaying recommender parameters
**Line  240** – Load  to display the various parameters used in an Item based Collaborative Filter (IBCF). 
**Line  245** – Load  to implement a recommender model using IBCF on the training dataset.
###### 9.2	Applying recommender system on the dataset
**Line  251** – Implementation of the “ predict function ()” to visualize the top 10 recommended movies to a user to specify the number of films to each user.
**Line  261** – Load  to output top 10 movies in the dataset for the first user.

# Check "Descriptive Statistics of Movie Recommender Results,pdf" to view analysis of results.
