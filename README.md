# Bank Marketing Campaign Analysis

## Overview

This project analyzes a bank marketing dataset to predict whether a client will subscribe to a term deposit. The dataset includes various features related to the client's personal and contact information, as well as the results of previous marketing campaigns.

## Dataset

The dataset used is the `bank-additional-full.csv`, which is a comprehensive version of the bank marketing dataset. It contains the following columns:

- **age**: Age of the client
- **job**: Type of job
- **marital**: Marital status
- **education**: Level of education
- **default**: Whether the client has credit in default
- **housing**: Whether the client has a housing loan
- **loan**: Whether the client has a personal loan
- **contact**: Type of communication used for the contact
- **month**: Last contact month of the year
- **day_of_week**: Last contact day of the week
- **duration**: Duration of the last contact
- **campaign**: Number of contacts performed during this campaign
- **pdays**: Number of days since the client was last contacted from a previous campaign
- **previous**: Number of contacts performed before this campaign
- **poutcome**: Outcome of the previous marketing campaign
- **emp.var.rate**: Employment variation rate
- **cons.price.idx**: Consumer price index
- **cons.conf.idx**: Consumer confidence index
- **euribor3m**: Euribor 3 month rate
- **nr.employed**: Number of employees
- **y**: Whether the client subscribed to the term deposit (target variable)

## Data Exploration

### Data Loading and Inspection

- Loaded the dataset and performed an initial inspection to understand the structure and content.

### Missing Values

- Checked for missing values; none were found.

### Descriptive Statistics

- Examined summary statistics for numerical features.

### Class Distribution

- Analyzed the target variable distribution to see the balance between 'yes' and 'no' subscriptions.

### Age Distribution

- Compared the age distribution of clients who subscribed ('yes') versus those who did not ('no').

## Data Preprocessing

### Balancing the Dataset

- To address class imbalance, a random sample of 4640 records was taken from the majority class ('no') to match the number of records in the minority class ('yes').

### Categorical Encoding

- Used LabelEncoder to convert categorical variables into numerical values.

### Normalization

- Applied MinMaxScaler to scale numerical features to a range [0, 1].

### Feature Correlation

- Computed and visualized the correlation matrix to understand the relationships between features.

## Model Evaluation

Trained and evaluated several classifiers to predict the likelihood of subscription:

- **SVM (Support Vector Machine)**: Achieved an accuracy of 83.998%
- **Logistic Regression**: Achieved an accuracy of 83.782%
- **K-Nearest Neighbors**: Achieved an accuracy of 86.369%
- **Decision Tree Classifier**: Achieved an accuracy of 82.489%
- **Random Forest Classifier**: Achieved an accuracy of 86.261%
- **Gaussian Naive Bayes**: Achieved an accuracy of 77.209%

The K-Nearest Neighbors and Random Forest models showed the highest accuracy in predicting client subscription.

## Conclusion

The analysis demonstrates the effectiveness of various machine learning algorithms in predicting whether a client will subscribe to a term deposit. The K-Nearest Neighbors classifier and Random Forest classifier performed the best, indicating their robustness in handling the given dataset.

Conclusion
The analysis demonstrates the effectiveness of various machine learning algorithms in predicting whether a client will subscribe to a term deposit. The K-Nearest Neighbors classifier and Random Forest classifier performed the best, indicating their robustness in handling the given dataset.
