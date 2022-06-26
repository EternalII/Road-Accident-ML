## Road-Accident-Prediction through Machine Learning

# Intro
This is a machine learning project to predict severe road accidents for Data Science course in HiT.
All data taken from the מאגר הנתונים הממשלתי https://data.gov.il/

# The Data
We are using the ITM standard for coordinates to ensure location accuracy and consistency with the data.
The accident severity level is based on 3 labels: 1 to 3, where 1 is most severe and 3 is least severe
The government website includes more data such as time, month, police file and more. Most of these data is handled almost blindly, where instead we rely on corr() function to find correlated features so we can remove them later.

# Goal
The goal of this project is to predict severe accidents based on specific locations picked through the ITM coordinates. The machine will learn from the available data, and predict the next possible accident.

# Results
So far the data's accuracy is set at 80%, which is good enough but not perfect. The best algorithm was the decision tree, which showed only about 0.9% improvement.

