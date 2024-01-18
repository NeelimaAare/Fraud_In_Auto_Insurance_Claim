# Fraud-in-auto-insurance-claims
Auto insurance fraud occurs when people or organized groups intentionally make false or exaggerated claims for damages, injuries, or theft related to their vehicles. This deceptive behavior poses a major challenge for insurance companies, resulting in higher costs and increased premiums for all policyholders. To combat this issue, detecting and preventing auto insurance fraud necessitates the use of advanced data analytics, thorough investigations, and cutting-edge fraud detection technologies. By employing a combination of these strategies, insurance companies can safeguard against fraudulent activities and mitigate the financial impact on honest policyholders.

# Data Pre processing and EDA
The datasets, including train_demographics, train_claim, train_policy, train_vehicle, test_demographics, test_claim, test_policy, test_vehicle, train, and test, have been successfully loaded. To provide a comprehensive overview, we displayed the head, data types, shape, info, descriptive statistics, and the count of missing values for each attribute in every CSV file.

Visualizations were employed to gain insights into the dataset columns. The next steps involved addressing missing values by utilizing mean, median, and mode imputation. Outliers were treated using the Interquartile Range (IQR) method. To facilitate machine learning model building, categorical-to-numerical type conversion was executed through Label Encoder.

Correlations between columns were examined to understand relationships within the data. Subsequently, the train and test datasets were merged based on the 'Customer_Id' attribute to create final training and testing data. Feature scaling was implemented by fitting and transforming the data, ensuring consistency in scale.

In addition, a decision tree was employed to identify the top 20 features, providing valuable insights into the most influential factors for the model. This comprehensive data preprocessing and transformation process lays the foundation for building a robust machine learning model for further analysis and predictions.

# Model Building
In the process of building a fraud detection model, 'X' has been defined to encompass all features from the training data except the 'ReportedFraud' column, while 'y' contains the corresponding 'ReportedFraud' labels. This standard setup is crucial for training classification models, with 'X' serving as input features and 'y' as the target variable for the model to learn the relationship between features and fraud labels.

To assess model performance, a train-test split was executed with a size of 0.3. Subsequently, Logistic Regression, K Nearest Neighbour, Decision Tree, Naive Bayes, and Random Forest classification models were constructed for fraud detection. The evaluation metric used was the F1 score, providing a balanced measure of precision and recall.

To enhance model performance, hyperparameter tuning was conducted on Decision Tree Classifier, Logistic Regression, KNN, and Random Forest models using GridSearchCV. This optimization process led to an improvement in the model's predictive capabilities.

The best-performing model's prediction results, along with Customer IDs, were saved in a CSV file. This holistic approach ensures the development of an effective fraud detection model, combining diverse machine learning algorithms, thorough evaluation metrics, and fine-tuning for optimal results.



# Advantages of Automated Fraud Detection Systems

1. Improved Fraud Detection:
Automated systems enhance fraud detection capabilities by swiftly analyzing vast datasets and identifying suspicious patterns. This proactive approach helps in early detection and mitigation of fraudulent activities.

2. Time and Cost Efficiency:
Automation significantly reduces the time and resources required for fraud detection. With rapid data processing and real-time analysis, organizations can efficiently allocate resources, ultimately leading to cost savings.

3. Increased Accuracy:
Automated fraud detection systems leverage advanced algorithms and machine learning models, resulting in higher accuracy compared to traditional manual methods. This accuracy minimizes false positives and ensures that genuine transactions are not mistakenly flagged as fraudulent.

4. Consistency and Objectivity:
Automated systems provide consistent and objective evaluations by applying predefined algorithms uniformly. This consistency eliminates human biases and ensures a fair and standardized approach to fraud detection.

5. Scalability:
Automated systems can easily scale to handle increasing data volumes and growing complexities in fraudulent activities. This scalability allows organizations to adapt to evolving threats and maintain effective fraud detection measures.

In summary, the adoption of automated fraud detection systems offers a range of benefits, including improved accuracy, time and cost efficiency, consistent and objective evaluations, and scalability to meet the dynamic challenges of fraud prevention.

