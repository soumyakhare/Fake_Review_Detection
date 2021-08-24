# fake-review-detection
This project primarily aims to classify fake and true reviews from the YELP dataset.
We aim to understand the various indicators that are used by current systems in flagging fake reviews. We also aim to identify new features that may assist this task. For this problem efficiency is not the most important aspect but accuracy is. And so the second goal of our project is to try out different machine learning algorithms and determine their extent of correctness. Finally we aim to report our findings with respect to combinations of features and algorithms that work with highest accuracy.

## Step 1:

The feature extraction process implemented in "Feature_Extraction.ipynb" and "SWM_UserFeatureExtraction_ModelTraining.ipynb" files which extracts the following 17 features and exports it to csv file:
1. polarity
2. subjectivity
3. wordCount
4. stdrating
5. clusterid
6. meanSimilarity
7. varOfSimilarity
8. meanRating
9. numberOfReviews
10. avgNoOfWords
11. totalReviews
12. isSingleton
13. posReviewRatio
14. negReviewRatio
15. avgNoOfReviews
16. maxNoOfReviews
17. dateVariance

## Step 2:
The feature importance and feature analysis through visualizations implemented in "Visualization.ipynb"

## Step 3:
The model training, testing and reporting model perfomrance report.
The file "SWM_UserFeatureExtraction_ModelTraining.ipynb" covers model training of random forest classifier using random sampling, random forest classifier using StratifiedK-fold cross validation, naive bayes classifier using Stratified-kfold cross validation.
The file "ANN.ipynb" implements a Artificial Deep neural network model and produces the performance measures and accuracy separately for each of the two classes.
The file "XGB&DecisionTree.ipynb" implements weight based gradient boosting and decision tree models and display the performance measures.

## Step 4:
After the model training, the file "Feature_Importance.ipynb" implements Eli5 which finds feature importance post model training and then displays the importance of each feature used in the training.
