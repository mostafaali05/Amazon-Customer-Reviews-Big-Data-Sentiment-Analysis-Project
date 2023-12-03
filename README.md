# Sentiment Analysis on Amazon US Customer Reviews Project

## Project Overview

This project aims to perform sentiment analysis on the Amazon US Customer Reviews dataset. The goal is to extract meaningful insights from customer feedback and explore various aspects of customer sentiment towards products on Amazon.com. This analysis can help businesses and researchers understand customer needs better and potentially improve product recommendations and customer experience.

## Dataset Description

The dataset used is the Amazon Customer Reviews dataset, also known as the Product Reviews dataset. It is a collection of customer feedback on Amazon.com, spanning over two decades and consisting of over a hundred million reviews. The dataset is available on Kaggle and can be accessed via this link: [Amazon US Customer Reviews Dataset](https://www.kaggle.com/datasets/cynthiarempel/amazon-us-customer-reviews-dataset?select=amazon_reviews_multilingual_US_v1_00.tsv).

Key attributes of the dataset include:
- Review IDs and Customer IDs
- Product IDs and categories
- Star ratings and review texts
- Helpful votes and total votes
- Verified purchase indicator and other relevant metadata

## Objectives

1. **Binary Classification of Sentiment**: Classify reviews as positive or negative based on their content and star ratings.
2. **Keyword Analysis**: Identify keywords correlating with positive or negative sentiments.
3. **Temporal Trend Analysis**: Examine how sentiments vary over time across different product categories.
4. **Product Recommendation Prediction**: Predict other products that customers might like based on their reviews and ratings.
5. **Duplicate and Anomaly Detection**: Identify duplicate reviews or anomalies that could indicate spam or fake reviews.

## Methodology

### Data Acquisition and Preprocessing
- Data was downloaded from Kaggle and processed using Python and PySpark.
- Preprocessing involved handling missing values, duplicates, and data normalization.

### Exploratory Data Analysis (EDA)
- EDA was conducted using Databricks, focusing on understanding the distribution of ratings, the presence of null values, and other key statistics.
- Visualization included bar plots, pie charts, and heatmaps to uncover patterns in the data.

### Feature Engineering
- Text data from reviews was tokenized, and stopwords were removed.
- Features were vectorized using techniques like HashingTF and IDF.
- Data was transformed into a format suitable for machine learning models.

### Modeling
- A Logistic Regression model was implemented to predict the sentiment of a review.
- The model's performance was evaluated using metrics like accuracy, precision, recall, and F1 score.
- ROC curves were plotted to assess model performance.

### Model Optimization
- Grid Search was used for hyperparameter tuning.
- The best model was selected based on the ROC score.

### Visualization
- Various plots were created to visualize actual vs. predicted results, confusion matrices, and ROC curves.

## Tools and Technologies
- Python, PySpark, Hadoop, Pandas, Numpy
- Amazon EC2, Amazon S3, Databricks
- Kaggle API
- Matplotlib, Seaborn for visualizations

## How to Run the Project

1. **Set Up Environment**: Ensure you have Python and Spark installed.
2. **Clone Repository**: Clone this repository to get the necessary code and notebooks.
3. **Load Data**: Download the dataset from Kaggle and store it in an accessible location.
4. **Run Notebooks**: Execute the Jupyter notebooks in order, starting from data acquisition to modeling.

## Future Scope

- Extend analysis to include more complex models like Neural Networks or BERT for deeper sentiment analysis.
- Incorporate more nuanced sentiment classification (e.g., neutral, mixed).
- Explore the impact of reviews on product sales.

## Contact

- **Name**: Mostafa Murshad Ali
- **Emails**: 
  - mostafamurshad.ali@baruchmail.cuny.edu (school)
  - mostafamurshadali@gmail.com (personal)
- **LinkedIn**: https://www.linkedin.com/in/mostafa-murshad-ali/

---

_
