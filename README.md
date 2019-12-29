# Machine Learning 
Logistic Regression,

In  this assignment,I learnt how  to apply logistic regression  on  a  small  dataset  with limited number of features (or entries) to predict which binary class each sample belongs to as shown in the figure.

Preparation: First  you  will  need  to download the  “hw1_dataset.csv”  fileincluded  with  this  homework assignment. This is a 250 x 7 dataset where there are 250 samples (observations) of 6 features (x1, x2, ..., x6) and 1 binary class label (y). Each feature column’s label is indicated at the top in the CSV file.

Objective: We  want  to  predict label “y”,from different combinations of  the  6  features  provided.  Select  4 different  combinations,  you  will  be  calculating  the  results  for  these  4  combinations  you  have selected.Example: (x1, x3, x5), (x1, x2, x3, x4, x5, x6), (x1, x2, x4, x6), (x2, x3, x4, x6)

Training: You will apply 5-fold cross validation as we discussed in class.You need to shuffle the dataset and divide it into 5 equal folds of 50 samples each.  You then choose 1 fold for testing,3 folds for training,and1  fold  for validation  (early-stopping)each  time  you  train  and  test  your  algorithm, doing this 5 times for each of the 5 folds.Train a logistic regression model with gradient descent using the training setfor each of the feature  combinations  you  have  selected,  4  models  in  total.You  will  use MSE as  your loss function. Stopping condition for training will be a maximum of 100 iterations or when MSE stops improving for 5 iterations in a rowfor the validation set, whichever happens first.You will have to select suitable hyperparameters.
(a)Plot  MSE  against the iteration  count,  for  training  and  validation  sets  on  the  same  plot.Display each fold  as a separate trace, 5traces each for training and validation.You will have to plotthisfor each of the 4 models separately and display them on the same figure as subplots on a 2x2 pattern. Here is a tutorial on subplots, with a lot of examples:Figure 1: Logistic Regression Model
https://matplotlib.org/api/_as_gen/matplotlib.pyplot.subplot.html

Testing: You will test the classification accuracy of the logistic regression models you have trained on thetest set. (b)Plot the classification accuracy against the iteration count for each of the 4 models on the same  figure  as  subplots  on  a  2x2  pattern. Displayeach  fold  as  a separate trace,5traces total.
