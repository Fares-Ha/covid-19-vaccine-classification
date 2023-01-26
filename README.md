# covid-19-vaccine-classification

## Intro

in this project the goal is to classify arabic tweets which are people opinions about covid-19 vaccination collected form tweeter, there are basicly two classes: 

0- against covid-19 vaccine
1- with covid-19 vaccine

## Data Set
The Data set I used in this model is collected from twitter based on people opinion's about covid-19 vaccination in [Arabic],I used different data cleaning methods to our Data then apply the methods that gives the best cleaning result.

## Models
In this project I used different models of machine learning and deep learning models.

the Baseline model was:logistic regression with bag of words with no preprocessing methods applied on Data.

accuracy :0.580


{2->8} logistic regression with bag of words each with different preprocessing method to find the best preprocessing method that affect more.

accuracy :{0.578,0.594,0.580,0.577,0.578,0.499,0.531}


{9} logistic regression with bag of words each with the best resulting preprocessing methods.

accuracy :0.592


{10} TF-IDF with model {9}.

accuracy :0.620


{11} multinominalNB with TFidfTransformer with no preprocessing methods applied on the data.

accuracy :0.634


{12} deep nueral network with tfidf with the best resulting preprocessing methods.

accuracy :0.594


{13} add Embedding layer to model {12} with the best resulting preprocessing methods.

accuracy :0.559


{14} add Embedding layer and maxpooling layer to model {12} with the best resulting preprocessing methods.

accuracy :0.567


{15} add CNN layer to model {12} with the best resulting preprocessing methods.

accuracy :0.506
