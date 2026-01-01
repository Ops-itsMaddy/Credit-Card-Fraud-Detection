**### Credit Card Fraud Detection**


This project implements a machine learning model to identify fraudulent credit card transactions. Given the highly imbalanced nature of fraud datasets, this project utilizes under-sampling techniques to build a balanced training set and employs Logistic Regression for classification.

**📌 Project Overview**


The goal of this project is to detect fraudulent transactions (Class 1) from legitimate ones (Class 0). The dataset contains transactions made by credit cards, where most transactions are normal, and only a small fraction are fraudulent.

**📊 Dataset Description**


The model is trained on a dataset containing 31 columns:

Time: Number of seconds elapsed between this transaction and the first transaction in the dataset.

V1-V28: Result of a PCA transformation to protect user identity and sensitive features.

Amount: Transaction amount.

Class: Target variable (0 for Legit, 1 for Fraudulent).

Data Distribution
Legit Transactions: 284,315

Fraudulent Transactions: 492

Status: Highly Unbalanced

**🛠️ Technologies Used**


Python 3.x

Pandas & NumPy: For data manipulation and analysis.

Scikit-learn: For model building, data splitting, and evaluation.

Jupyter Notebook/Google Colab: For interactive development.

**🚀 Workflow**


Data Loading: Importing the dataset using Pandas.

Data Analysis: Checking for missing values and analyzing the distribution of legit vs. fraud transactions.

Preprocessing:

Separating the data into two classes.

Performing Under-sampling by creating a sample dataset of 492 legit transactions to match the number of fraudulent ones.

Model Training: Training a Logistic Regression model on the balanced dataset.

Evaluation: Measuring accuracy on both training and testing data.

Predictive System: Building a system to input transaction features and predict if it is legit or fraud.

**📈 Performance Results**


The model achieved the following accuracy scores:

Training Data Accuracy: ~94.79%

Testing Data Accuracy: ~93.40%