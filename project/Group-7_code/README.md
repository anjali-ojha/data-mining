
## File Descriptions

Authors -  Group 7 (Akanksha Tyagi, Anjali Ojha, Srushti Doshi, Sakshi Mukkirwar) 

As the data is very big we are not submitting the data here. The data can be downloaded from the below link.

Dataset path = https://www.kaggle.com/competitions/ieee-fraud-detection/data 

```angular2html
Dataset Description
In this competition you are predicting the probability that an online transaction is fraudulent, as denoted by the binary target isFraud.

The data is broken into two files identity and transaction, which are joined by TransactionID. Not all transactions have corresponding identity information.

Categorical Features - Transaction
ProductCD
card1 - card6
addr1, addr2
P_emaildomain
R_emaildomain
M1 - M9
Categorical Features - Identity
DeviceType
DeviceInfo
id_12 - id_38
The TransactionDT feature is a timedelta from a given reference datetime (not an actual timestamp).

You can read more about the data from this post by the competition host.

Files
train_{transaction, identity}.csv - the training set
test_{transaction, identity}.csv - the test set (you must predict the isFraud value for these observations)
sample_submission.csv - a sample submission file in the correct format
```

1- feature_generation.ipynb  - This notebook focuses on feature engineering for the fraud detection dataset. It includes methods to create new features, transform existing ones, and prepare data for modeling.
ieee-fraud-detection

2- modeling.ipynb  - This notebook is dedicated to building, training, and evaluating machine learning models. It includes steps such as hyperparameter tuning, model evaluation, and generating predictions.

3- project_eda_1.ipynb  - The first part of exploratory data analysis (EDA), focusing on understanding the dataset. It includes visualizations, distributions, and missing data analysis.

4 - project_eda_2.ipynb - The second part of EDA, performing detailed analysis of specific features, correlations, and temporal trends. This notebook may include advanced visualizations and feature-specific investigations.

5 - project_eda_3_device.ipynb - Focused on analyzing device-related features in the dataset. It likely includes insights into device types, operating systems, browser versions, and screen resolutions.

6 - requirements.txt - A text file containing the required libraries and dependencies for running the code. You can install them using pip install -r requirements.txt.

7- dataset_readme.md - this file have information about the dataset.

## Instructions

```
To run this code 
    1-  download the dataset from the link https://www.kaggle.com/competitions/ieee-fraud-detection/data
    2-  Extract the dataset and place it in the same directory as the notebooks
    3-  Install the required libraries using the command pip install -r requirements.txt
    4-  based on the current folder the data should be at path 
        ./ieee-fraud-detection/sample_submission.csv
        ./ieee-fraud-detection/test_identity.csv
        ./ieee-fraud-detection/test_transaction.csv
        ./ieee-fraud-detection/train_identity.csv
        ./ieee-fraud-detection/train_transaction.csv
        ./ieee-fraud-detection/transaction.csv
        
    5-  Open the notebooks in jupyter and run it

```

jupyter notebook
Run the notebooks in the following order for reproducibility:
    project_eda_1.ipynb
    project_eda_2.ipynb
    project_eda_3_device.ipynb
    feature_generation.ipynb
    modeling.ipynb