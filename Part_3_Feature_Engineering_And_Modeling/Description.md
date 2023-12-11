# Feature Engineering, and Modeling with Amazon Reviews Data

This repository contains the code and documentation for the Cleaning, Feature Engineering, and Modeling phases of a data analysis project using the Amazon Reviews dataset. This project is structured in a way to efficiently handle and analyze large-scale data using Databricks and AWS S3.

## Project Structure

The project is divided into two main parts:

1. **Cleaning**: The initial phase involves cleaning the Amazon Reviews dataset and storing it in the AWS S3 `amazon-reviews-ma/raw` folder in Parquet format.

2. **Modeling**: After cleaning, the data is used for modeling purposes. The cleaned data is retrieved from the `raw` folder, processed through feature engineering, and the resultant data is stored in the `amazon-reviews-ma/trusted` folder.

## Cleaning Process

- **Dataset**: The dataset used for this phase is `amazon_reviews_multilingual_US_v1_00.tsv` (3.8 GB).

- **Data Cleaning Steps**:
  - Import necessary libraries like pandas, seaborn, sklearn, numpy, boto3, and pyspark.
  - Set up AWS credentials and configure Hadoop to interact with S3.
  - Load the dataset using Spark, perform initial exploratory analysis, and clean the data.
  - This includes removing duplicates, handling null values, and extracting ASCII-only text.
  - The cleaned data is then written back to S3 as a Parquet file.

## Feature Engineering and Modeling

### Model 1

- **Goal**: Predict whether a product rating is 'good' (greater than 3) or 'bad' (less than or equal to 3).
- **Process**:
  - Feature engineering on `clean_review_headline` and `clean_review_body` using tokenizers, stop words remover, and hashing.
  - Logistic Regression model is used for prediction.
  - Performance is evaluated using metrics like accuracy, precision, recall, F1 score, and ROC AUC.

### Model 2

- **Addition**: Incorporates the `product_category` column, requiring the combination of multiple files.
- **Process**:
  - Similar to Model 1 but includes OneHotEncoding for the `product_category`.
  - Combines data from multiple product categories for a more comprehensive model.
  - Evaluation metrics are similar to Model 1.

## Summary

- The project demonstrates the effective use of Databricks and AWS S3 for handling large datasets.
- The Logistic Regression model provides satisfactory results in predicting product ratings.
- Both models show promising performance with scope for further improvement and scalability.

---
