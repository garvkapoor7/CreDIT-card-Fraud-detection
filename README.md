# CreDIT-card-Fraud-detection
The model is a Logistic Regression classifier designed to detect credit card fraud by training on balanced data and evaluating its performance using accuracy metrics.


1. Data Preprocessing and Preparation:
Loading and Cleaning: The model starts by loading the credit card fraud dataset and performs initial data cleaning, such as removing duplicates and handling missing values.
Feature Selection: The 'Time' feature is dropped, assuming it's not relevant for fraud detection.
Class Imbalance Handling: To address the imbalance between legal and fraudulent transactions, the data is undersampled by randomly selecting a subset of legal transactions to match the number of fraudulent ones.
2. Model Training:
Logistic Regression: A logistic regression model is chosen as the classification algorithm. This is a suitable choice for binary classification problems like fraud detection.
Training on Undersampled Data: The model is trained on the undersampled dataset, which helps to prevent the model from being biased towards the majority class (legal transactions).
3. Model Evaluation:
Prediction on Testing Data: The trained model is used to make predictions on the testing data, which was held back during training to evaluate the model's performance on unseen data.
Accuracy Measurement: The accuracy score is calculated to assess the model's overall performance. This metric measures the proportion of correct predictions out of the total predictions.
4. Addressing Class Imbalance (Optional):
SMOTE: The code also explores the use of SMOTE (Synthetic Minority Over-sampling Technique) as an alternative to undersampling. SMOTE generates synthetic data points for the minority class (fraudulent transactions) to balance the class distribution. This can help improve the model's performance in cases where undersampling might not be sufficient.

DATASET LINK : https://drive.google.com/file/d/1PGJgjmGAfR-uan792TSD_RUAEYw2T63z/view?usp=drive_link
