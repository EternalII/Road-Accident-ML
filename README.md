[Show Map](https://eternalii.github.io/Road-Accident-ML/map.md){: .btn}

# Road Risk prediction through Machine Learning

## Intro
This is a machine learning project for Data Science course in HIT, where we are tasked to predict results using Machine Learning. We chose to focus on predicting of severe road accidents as the best way to avoid an accident is not to be in one in the first place.

All data taken from the [מאגר הנתונים הממשלתי], their website link is https://data.gov.il/

## The Data
We are using the ITM standard for coordinates to ensure location accuracy and consistency with the data.
The accident severity level is based on 3 labels: 1 to 3, where 1 is most severe and 3 is least severe.
The government website includes more data such as time, month, police file and more. Most of these data is handled almost blindly, where instead we rely on corr() function to find correlated features so we can remove them later.

## Goal
The goal of this project is to predict severe accidents based on specific locations picked through the ITM coordinates. The machine will learn from the available data, and predict the next possible accident.

## Results
So far the data's accuracy is set at 80%, which is good enough but not perfect. The best algorithm was the decision tree, which showed only about 0.9% improvement.
For clarification, by pointing at a remote area the machine will return "3", meaning if a crash takes place there, it's most likely not that severe. On the other hand, point at a road with nearby incidents, you might get "2" or "1" as a result, which means the accident will be severe.

## The Code
We are using Anaconda distribution for the Python Code. The libraries being used in this project are Pandas, Scikit-learn, Matplotlib and Seaborn.

* Pandas for data tables and manipulating that data
* Scikit for machine learning
* Matplotlib and Seaborn for drawing plots to display that data
