![alt text](https://github.com/josephimathias/Predicting_Hits_Project/blob/master/images/title.png)
# Predicting Hits - Categorizing Balls-in-Play in MLB
## Joey Mathias and Daniel Torres

This project involves conducting various categorical analyses to predict hit type given over 50 potential features. Please see the slides that accompany this project [here](https://github.com/josephimathias/Predicting_Hits_Project/blob/master/slides.pdf).

### Goal
Our goal was to determine whether a ball put into play would result in a single, double, triple, home run, sacrifice bunt, or sacrifice fly. Our potential features included what type of pitch was thrown, the angle at which the ball was hit, and many others.

Here are the balls in play that we investigated, grouped by "launch angle" and "launch speed":
![alt text](https://github.com/josephimathias/Predicting_Hits_Project/blob/master/images/original_clusters.gif)

### Process
* We selected 36 of 89 features for experimentation
* We balanced data using SMOTE
* We train/test split our data and ran: decision trees, random forest, KNN, Gradient Boost, XGBoost
* We visualized our errors

### Results
We correctly predicted the hit-type for **83%** of the balls put into play.
Here is the resulting confusion matrix:
![alt text](https://github.com/josephimathias/Predicting_Hits_Project/blob/master/images/confusion_matrix.png)

It is clear from the matrix that the model did well with some types of hits and not others.
Here is a graphical representation of our test home runs, with incorrect predictions in yellow:
![alt text](https://github.com/josephimathias/Predicting_Hits_Project/blob/master/images/true_home_runs.gif)

### Files in Repository:
* README.md - Joey
* Technical_Notebook.ipnby - This file contains our entire process including feature selection, modeling, and visualization - Joey and Daniel
* slides.pdf - This file contains the project slides - Joey and Daniel
* images - This folder contains images including illustrative gifs and this README's header - Joey
* data - This folder contains the data that we analyzed, downloaded from Baseball Savant  - [BaseballSavant](https://baseballsavant.mlb.com)
