# Naive Bayes Classifier - Machine Learning Project

*Overview*

*Hi there! This project is a Jupyter Notebook where I explore and compare different machine learning algorithms, with a special focus on Naive Bayes. I also try out other models like Logistic Regression and K-Nearest Neighbors (KNN). The goal? To figure out which algorithm performs best on a dataset that contains missing values. Throughout the project, I use different techniques to handle these missing values and see how each impacts the model’s performance.*

## **Algorithms I used:**

Naive Bayes – The star of the show!

Logistic Regression – A popular linear classifier.

K-Nearest Neighbors (KNN) – A simple, non-parametric algorithm.


For each of these algorithms, I tried different imputation methods to fill in the missing data and then trained the models on the preprocessed dataset.

## **Project Breakdown**

*1. Data Preprocessing*
The dataset has some missing values, so I use a few different techniques to fill them in:

Simple Imputer (SI): Replaces missing values with the mean, median, or most frequent value.
Iterative Imputer: Uses models to predict and fill in missing values.

KNN Imputer: Fills missing values based on similar neighbors.

*2. Implementing the Models*

Once the missing data is handled, I implement and train each model:

Naive Bayes: This is a probabilistic model that applies Bayes' Theorem for classification.

Logistic Regression: A classic linear algorithm for binary classification.

KNN: Looks at the nearest data points to make its predictions.

*3. Evaluating the Results*

To compare the models, I use accuracy as the main metric. The results? Naive Bayes generally performs the best, but Logistic Regression with iterative imputation actually scored higher (92%) in one case. On the flip side, KNN combined with KNN imputation had the weakest performance, making it the least compatible combo.

*4. Key Findings*

The notebook finishes with some interesting insights:


Naive Bayes is reliable across different imputation methods, consistently achieving strong accuracy scores.

Logistic Regression with the Iterative Imputer was a standout performer, beating Naive Bayes in one scenario with an impressive 92% accuracy.

KNN didn’t perform as well, especially with the KNN Imputer. That method actually produced the worst accuracy scores.


## **Conclusion**
From this project, I’ve learned that Naive Bayes is a great option when dealing with incomplete datasets and different imputation techniques. The exception here is Logistic Regression paired with the Iterative Imputer, which yielded the highest accuracy in certain cases. On the other hand, KNN struggled, particularly when used with the KNN imputer.
