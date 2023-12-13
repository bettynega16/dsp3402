
![UTA-DataScience-Logo](https://github.com/bettynega16/dsp3402/assets/111395189/7a47be87-27e5-4410-a606-a5950979da74)

## EMI Music DS Hackathon
 This repository hold an attempt to apply Decision tree classifier to predict if user's rating for particular song after hearing it for the first time.

 ## Overview
 The task is to use the csv files provide that describe Users, Artist, and tracks to predict the rating of a particular song a user just heard. The approach in this repository formulates the problem as classification task, using Decision tree as a model with user’s and Artist information as a input.  The model was able to use 8o% of the data for predication but the best accuracy at the time is 3.5%.

 ## Summary of Workdone
### Data
 
 Input is  train.csv, test.csv, words.csv, Userkey.csv, user.csv, Sample.r, logo_greenplum_main.png. In total there was 11 files. Output is test.csv. In total the size of the Data was 46.44 MB.

 There was no processing or cleanup done. But in the user's file the participants are asked 19 questions but I only used one because that is the most relevant.

### Data Visualization
![download](https://github.com/bettynega16/dsp3402/assets/111395189/a4b97a7b-fc88-4ae6-a59b-0f81f5ef60ac)
   compared the Artist value count and Rating value count.
   
![download](https://github.com/bettynega16/dsp3402/assets/111395189/ff0eec71-a07a-415b-b1de-bb1ae345ac11)
   Shows the relation between question 1: I enjoy actively searching for and discovering music that I have never heard before and user’s opinions about music.

   
 ### Problem Formulation 
 
 The input was the userkey and user csv file. In this file it had information about the user’s age, gender, Jobs, etc. The output is to predict if the user will like a certain song based of their information. The model I used is Decision Tree classifier. Decision Trees are often used for classification tasks where the goal is to predict the class or category of the target variable based on the input features.

 ### Training 

 The first thing I did was split the train data 80% training and 20% testing using Decision Tree Classifier.  I used the train test split to split the train file in to X_train, X_test, y_train, y_test. After that I used model fit to fit the X_train and y_train and predict X_test. In this portion of the project I did not run in to a problem.

### Performance Comparison 

 I only used the accuracy score metrics from scikit learn, to the measure the accuracy of the model. I moved around the input (x) and output (y) because the accuracy level was very low.

 ### Conclusion 

 I used Decision Tree classifier and thought it would have worked if I was able to minimize my input to specific things. Based of the accuracy I got (3.5%) I do not think I used the model correctly.

### Future Work

 I want to use the userkey csv instead of the train csv to train the model . I believe the data from this file would have made the accuracy rate bigger. I another thing I did not get to do was use the model Logistic Regressio so I did not get compare to Decison Tree Classifier.

 ## How to reproduce results 
 
 ### Overview of files in repository 

I started of by opening all the files that was given to me so I can visualize the information they provided. From there I made bar graphs and for each rows or comparing row to get more information. After I was able to understand the what the csv files provided I trained the data on Decision tree classifier.

### Software Setup
        import pandas as pd
        import numpy as np
        import matplotlib.pyplot as plt 
        from IPython.display import Image
        from matplotlib.ticker import MaxNLocator
        from sklearn.tree import DecisionTreeClassifier
        from sklearn.model_selection import train_test_split
        from sklearn.metrics import accuracy_score

### Data 
ON https://www.kaggle.com/competitions/MusicHackathon/overview, clic on the Data tab and you will see all 11 files listed there. You can click on each one inorder to view it and it also gives you a chocies to download it.

### Training 
The first thing you need to do is split your data in to two sets. It is best to use 80% for training and 20% for testing, If you do not do this the accuracy will be low. when you split the model in to X (input) and Y (output). In this case Y is going to be the ratings and X is going to be User's informations.

## Citations
https://www.kaggle.com/competitions/MusicHackathon/overview
