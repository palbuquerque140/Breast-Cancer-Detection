# Breast Cancer Image Classification

## Overview 

This project is split in two different stages.
The first stage consists in developing a binary classification deep learning model to distinguish between Benign and Malignant tumors using histopathological images from BreaKHis dataset (~7,900 images with magnifications of 40x, 100x, 200x, and 400x)

The second stage consists in a multi class classification using the same images from the first stage, but this time the goal is to predict which type of cancer is the image displaying, between 8 different types used for training. 

OVerall, the main goal is to develop a model(s) that can assist in the accurate diagnosis of breast tissues 
by classifying images in both broad and detailed categories.

## Summary of Insights

In a binary classification cancer project, the most important metric to analyse would be the recall, as our aim is to minimize the number of false negatives, i.e, the cases where the model predicts a benign tumor when it is actually malignant. Nevertheless, accuracy is also an important metric and it should also be analyised. 

There were used several different techniques to counter the fact that the dataset was unbalanced, with maligant representing 68% of the data, so class weights to give more importance to the Benign Class as well as Data Augmentation to expose the model to the images in several different ways. Two models were trained and both performed quite similarly. The confusion matrix of both are displayed below:

![Binary Classification CM](Binary_Classification\results\Model_Comparison_CM.png)