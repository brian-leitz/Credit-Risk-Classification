# Credit-Risk-Classification
Using a dataset of historical lending activity from a peer-to-peer lending services company to build and evaluate, based on loan risk, a model that can identify the creditworthiness of borrowers.


# Credit Risk Classification Report

## Overview of the Analysis

## In this analysis, two supervised machine learning models were used to analyze the credit worthiness of borrowers from historical lending data:

## This data consists of historical lending activity from a peer to peer company. The purpose of this analysis is to use the data to build a supervised machine learning model to predict the credit worthiness of borrowers and classify each borrower as either a healthy loan or a high-risk loan. We start this analysis by importing the data into Jupyter Notebook and creating a dataframe. I then create the labels for the model, y, set from the "loan_status" column, then I create the features dataframe, x, from the remaining columns. At this stage in our process, we can see that the number of healthy loans significantly outweigh the number of high-risk loans. This means that the variation with regards to the accuracy when predicting our high-risk loans will be much greater and this may cause accuracy issues with our model. After going through the train, test, and split process, we then used a Logistic Regression model to fit our training data to. Next we make our predictions on the testing data labels using the testing feature data and our fitted model. After making our predictions, we then evalue the model's performance using an accuracy score, a confusion matrix, and a classification report. 

##    I then repeat this process with resampled data to see if our model can predict this data more accurately, starting with RandomOverSample to resample the data and confirm the labels have an equal number of data points. After repeating the process we used in our first model, we find that the model certainly fits better with the oversampled data, we can observe that the model is still predicting healthy loans at a very high accuracy, and high-risk loans are now showing a higher recall and accuracy score but still the model is not signficantly more precise than model one that used our original predicted data. 


## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

## * Machine Learning Model 1:
  * The model predicts the healthy loan to a very high precision, recall, and accuracy score significantly better then the high-risk loan. This would be a sign the the model is predicting the high-risk loans adequately but not quite well enough. Since high-risk loans are generally more unpredictable, we would want a higher precision and a higher recall score to be able to better predict the risk associated with those borrowers. 


## * Machine Learning Model 2:
  * This model uses resampled data, our results show an improved model with precision, recall, and accuracy scores for the model staying at a high score of 1.00, this model improves on our accuracy from the previous model, but still our precision has not made an improvement and still yeilding the same results. 

## Summary
* Our Second Machine Learning Model performed the best, we can see in the classsification report that our second model yielded a higher accuracy, high recall scores and averages, as well as high precision scores except that our high risk loan precision scores have still not improved. 
* It is still important to predict the healthy loan borrowers and this model does that however, accuracy on models is also important and this model has a higher accuracy score for our high-risk borrower. 
