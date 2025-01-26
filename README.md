# Data-science-portfolio

Problem Statement: 
     Our project focuses on customer segmentation 
     using advanced analytics to enhance
     business strategies.

Project Outcome: 
     The anticipated outcome is a sophisticated 
     customer segmentation model that provides 
     commercial value by optimizing marketing 
     efforts, increasing customer retention, and 
     driving revenue growth. 

     The dataset contains information about rom their consumers. The aim is to determine which class does a particular consumer belong to based on the several factors from their profile.

Attribute information:
 Invoice No: Invoice number. Nominal, a 6-digit integral number uniquely assigned to each transaction. If this code starts with letter 'c', it indicates a cancellation.
Stock Code: Product (item) code. Nominal, a 5-digit integral number uniquely assigned to each distinct product. Description: Product (item) name. Nominal.
Quantity: The quantities of each product (item) per transaction. Numeric.
Invoice Date: Invoice Date and time. Numeric, the day and time when each transaction was generated.
Unit Price: Unit price. Numeric, Product price per unit in sterling.
Customer ID: Customer number. Nominal, a 5-digit integral number uniquely 
       assigned to each customer.
Country: Country name. Nominal, the name of the country where each customer resides.
Age : The age of the consumer.
Gender : Gender of the consumer.
Salary : Salary of the consumer.

DROPPING REDUCTANT COLUMNS:
Dropping columns like Index, InvoiceDate which are not needed for the current analysis.

REMOVING DUPLICATES:
There were 196 rows which were identified as duplicate observations and were removed from the dataset.

TREATMENT OF NULL VALUES:
Identified and handled missing values by imputing with 
       mean/median/mode.
Mean and median for numeric columns and mode for categorical columns.

Data points outside a specified range are considered potential outliers. Typically, a common rule of thumb is to identify outliers as values lying below First Quartile Q1 
or above Third Quartile Q3.

Standard scaling :
 It involves transforming the data such that it has a mean of 0 and a standard deviation of 1. This process helps to remove the effect of the scale of the features, making them comparable and ensuring that each feature contributes equally to the analysis.

One hot encoding :
One hot encoding is a technique used in machine learning to convert categorical data into a numerical format, which can be used by various algorithms for model training.

Frequency Encoding :
Frequency encoding is a technique used in feature engineering to transform categorical variables into numerical representations based on the frequency of each category in the dataset. Instead of representing categories with arbitrary integer indices or binary vectors like one hot encoding, frequency encoding replaces each category with the count or frequency of occurrences of that category in the dataset.We have done Frequency encoding to categorical columns such as Description and StockCode.

LOGISTIC REGRESSION MODEL

Weighted F1 Score - Train : 0.69
Weighted F1 Score - Test : 0.70
Accuracy - Test : 0.70

The Decision Tree Model exhibit the highest performance on the training data, with F1 scores of 0.90 indicating strong predictive capabilities. This indicates that the model effectively captures the underlying patterns in the data and generalizes well to new observations.

Decision trees are inherently interpretable models, making it easier for stakeholders to understand the reasoning behind predictions.

While other models like KNN, Random Forest, and Gradient Boosting have been considered, the Decision Tree Model emerges as the top performer, balancing predictive accuracy and interpretability.

Based on the analysis, the Decision Tree Model stands out as the preferred choice for predicting the target variable.

 Its high performance, interpretability, and ability to capture important features make it a valuable tool for making informed business decisions. 

Additionally, the model's ability to generalize well to unseen data further strengthens its suitability for real-world applications.
