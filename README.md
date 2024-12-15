# Credit Card Fraud Detection
This project focuses on detecting fraudulent credit card transactions using machine learning algorithms. By leveraging historical transaction data, it builds a classification model to distinguish between legitimate and fraudulent transactions. The project addresses the class imbalance inherent in fraud detection datasets and incorporates hyperparameter tuning to optimize model performance.

## Features
- Data Exploration: Analysis of transaction patterns and distribution of fraud vs. legitimate transactions.
- Machine Learning Models:
- Logistic Regression
- Random Forest
- Decision Tree
- Hyperparameter Tuning:
- Optimized using RandomizedSearchCV for Random Forest and Logistic Regression.
- Model Evaluation: Metrics such as accuracy, precision, and recall to assess performance.
## Dataset
The dataset used for this project includes anonymized transaction data with the following features:

- Time: Time elapsed since the first transaction in the dataset.
- V1, V2, ..., V28: Principal Component Analysis (PCA)-transformed features.
- Amount: Transaction amount.
- Class: Target variable, where 1 indicates a fraudulent transaction and 0 indicates a legitimate one.
- The dataset used in this implementation can be obtained from Kaggle - Credit Card Fraud Detection Dataset.

## Requirements
The project uses the following Python libraries:
- numpy
- pandas
- scikit-learn
## Clone the repository:
git clone https://github.com/anandreddy05/Credit_Card_Fraud_Detection.git

## Methodology

## Data Preprocessing
- Splitting the dataset into training and testing sets.
- Balancing the dataset using techniques such as oversampling or undersampling (not explicitly shown but recommended for imbalanced datasets).
- Model Training and Evaluation

## Three machine learning models were trained:
 
- Logistic Regression: Achieved ~94.7% accuracy on the training set and ~96.9% on the test set after hyperparameter tuning.
- Random Forest: Achieved near-perfect accuracy on the training set and ~96.9% on the test set.
- Decision Tree: Achieved 100% accuracy on the training set but lower generalization accuracy on the test set (~93.9%).
## Hyperparameter Tuning
- RandomizedSearchCV was used to identify the best parameters for Logistic Regression and Random Forest models, optimizing for metrics like accuracy and generalization performance.
