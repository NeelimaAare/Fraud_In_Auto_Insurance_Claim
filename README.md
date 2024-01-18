# Fraud-in-auto-insurance-claims
Auto insurance fraud occurs when individuals ororganized groups intentionally submit false orexaggerated claims for damages, injuries, ortheft involving their vehicles. This type of fraudis a significant problem for insurancecompanies, as it leads to increased costs andhigher premiums for all policyholders. 
Detectingand preventing auto insurance fraud requires acombination of advanced data analytics,investigations, and fraud detection technologies.

# Data Pre processing and EDA
train_demographics, train_claim , train_policy , train_vehicle , train , test_demographics,
test_claim, test_policy, test_vehicle , test --> Loaded datasets.

Displayed head, data types, shape, info, descriptive statistics, missing values, counts for each
attribute in every csv files.

Visualisation performed on the columns and obtained insigthts.

Missing value treatment performed using mean, median and mode.
Outlier treatment performed using IQR method
Type conversion(From categorical to numerical) performed using Label Encoder.
Correlation between the columns displayed.

All the test and train datasets merged on Customer_Id attribute to get final training and testing
data to build the machine learning model.
Feature scaling performed by fitting and transforming the data.

Additionally top 20 featured displayed using decision tree feature importances.

# Model Building
'X' will contain all the features from the training_data DataFrame except the 'ReportedFraud'
column, and 'y' will contain the 'ReportedFraud' column values as the target labels. These
variables are then typically used for traied fning a classification model, where X is used as input
features, and y is used as the corresponding target variable for training the model to learn the
relationship between the features and the fraud labels.
Train-Test split performed with size of 0.3
Build Logistic Regression, K Nearest Neighbour , Decision Tree, Naive bayes and Random Forest
classification models for fraud detection.
Evaluation matrics --> F1 score obtained from all the above mentioned machine learning models.
Machine learning hyper parameter tuning performed on Decision tree classifier, Logistic
regression , KNN and Random forest models using GridSearchCV.
An increase in the model performance shown.
The best result model prediction results saved along with Customer Id in a CSV file.

# Advantages
1.Improved Fraud Detection

2.Time and Cost Efficiency

3.Increased Accuracy

4.Consistency and Objectivity

5.Scalability
