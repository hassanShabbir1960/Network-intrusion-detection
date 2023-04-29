# README.md

## Investigating the NSL-KDD Dataset
This Jupyter notebook provides a fundamental analysis of the NSL-KDD dataset, focusing on the following objectives:

1. Acquire a basic comprehension of the dataset.
2. Examine how the dataset could be employed to forecast network anomalies or intrusions.
3. Discuss essential principles of constructing machine learning models.

Throughout this exploration, we manually perform tasks that could be more efficiently accomplished using built-in functionalities in the scikit-learn library. This approach is taken to foster a deeper understanding of the processes involved and their rationale. We will explore the use of these built-in tools in a subsequent notebook.

## Modules Used
- NumPy
- pandas
- Matplotlib
- Seaborn
- itertools
- random
- scikit-learn

## Data
The dataset used in this notebook is the NSL-KDD dataset, which can be found at the following links:

- Training set: 'KDDTrain+.txt'
- Test set: 'KDDTest+.txt'

The NSL-KDD dataset can be downloaded from [Kaggle](https://www.kaggle.com/datasets/hassan06/nslkdd).


## Notebook Outline
1. Data Loading
2. Initial Data Transformations
3. Data Profiling
4. Feature Encoding and Splitting
5. Model Training and Evaluation
6. Database Implementation

## Model Training and Evaluation
The notebook includes the comparison of different classification models' performance, such as:

- Random Forest Classifier
- Logistic Regression
- K-Nearest Neighbors Classifier
- Decision Tree Classifier
- Gaussian Naive Bayes
- Multinomial Naive Bayes
- Bernoulli Naive Bayes

Performance metrics considered are:

- Accuracy
- Precision
- Recall
- F1 Score

Confusion matrices for each classifier are displayed using heatmaps.

## Database Implementation
The notebook includes an implementation of a database to store logs and alerts generated by the model. The database will provide a record of network traffic and any alerts generated, which will be useful for analyzing patterns of suspicious activity.

## Classifier Performance Comparison

| Classifier               | Accuracy | Precision | Recall  | F1 Score |
|--------------------------|----------|-----------|---------|----------|
| RandomForestClassifier   | 0.976542 | 0.977258  | 0.976542 | 0.975901 |
| LogisticRegression       | 0.787204 | 0.777808  | 0.787204 | 0.771578 |
| KNeighborsClassifier     | 0.971918 | 0.973584  | 0.971918 | 0.971988 |
| DecisionTreeClassifier   | 0.976364 | 0.977093  | 0.976364 | 0.975775 |
| GaussianNB               | 0.385475 | 0.566619  | 0.385475 | 0.259521 |
| MultinomialNB            | 0.446282 | 0.763515  | 0.446282 | 0.455304 |
| BernoulliNB              | 0.892833 | 0.902999  | 0.892833 | 0.896735 |

A comparison of various classification models based on their performance metrics (Accuracy, Precision, Recall, and F1 Score).
