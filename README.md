# Ml-project-predicting-default-on-payments-for-consumers

### Data
A data file titled data.csv contains all necessary data.
A text document titled desc.txt which contains descriptions for individual features present in the data.
The dataset encompasses financial data regarding consumer default on payments, as referenced by Yeh and Lien in 2009. Included within are 24 features encapsulating various parameters such as gender, marital status, age, and history of past payments. The binary-valued label "default payment next month" indicates whether the consumer defaulted on the subsequent month's payment. For a comprehensive understanding of the dataset, it is advisable to refer to desc.txt

### Implementation: 

In this project, the implementation was driven by the following pipelines in mind with two core components:

Feature Scaling: Given the broad range of raw values in a dataset, feature scaling aids in normalizing this variation to a common scale. The task involves experimenting with StandardScaler and MinMaxScaler from sklearn for data scaling.
Classification: The pipeline's second component is a classifier. LinearSVC, LogisticRegression, and KNeighborsClassifier classifiers are to be utilized in this assignment. The experiments is conducted including:

(a) For a LinearSVC classifier:
  Utilizing GridSearchCV to ascertain an optimal value for the regularization parameter C. Fitting the classifier on both scaled and unscaled data versions, reporting the estimator scores, and observing the impact of scaling on model performance.

(b) For a LogisticRegression classifier:
  Employing GridSearchCV to determine an optimal value for the “inverse of regularization strength” C. Fitting the classifier on both scaled and unscaled data versions, reporting the estimator scores, and observing the impact of scaling on model performance.

(c) For a KNeighborsClassifier classifier: Using GridSearchCV to find an optimal value for the “number of neighbors” n_neighbors. Fitting the classifier on both scaled and unscaled data versions, reporting the estimator scores, and observing the impact of scaling on model performance.

### Evaluation metrics: 

Accuracy, Macro and Micro-Averaged Precision and Recall, F1 Score

**Credits:** This project was part of group project and was completed together with Lorenzo Parma, Aleksandra Twardowska and Sushut Munje.

**References:** Yeh, I.-C. and Lien, C.-h. (2009). The comparisons of data mining techniques for the predictive accuracy of probability of default of credit card clients. Expert Systems with Applications, 36(2):2473–2480.
