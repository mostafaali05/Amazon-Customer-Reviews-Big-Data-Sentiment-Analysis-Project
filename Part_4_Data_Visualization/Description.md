# Data Visualization for Amazon Reviews Prediction Models

This repository contains the code and documentation for the Data Visualization phase of the Amazon Reviews sentiment analysis project. This phase focuses on visualizing the results and performance of the prediction models developed in the previous milestone.

## Overview

The visualizations are aimed at providing insights into the model's performance and predictions, using various graphical representations.

## Process

### Setting Up

- **Imports**: Required libraries include PySpark components, Matplotlib, Seaborn, and Pandas.
- **Model Loading**: The previously saved Logistic Regression model is loaded from an S3 path.

### Visualizations Created

1. **Actual vs Predicted Analysis**
   - A comparison of actual labels vs predicted labels using a countplot.
   - Highlights the model's accuracy in terms of prediction distribution.

2. **Confusion Matrix**
   - Visualizes the confusion matrix of the model to understand true positives, false positives, true negatives, and false negatives.
   - A heatmap is used for better clarity and understanding.

3. **ROC Curve**
   - Plots the Receiver Operating Characteristic (ROC) curve to evaluate the true positive rate vs false positive rate.
   - A measure of the model's ability to distinguish between classes.

4. **Precision-Recall Curve**
   - Illustrates the trade-off between precision and recall for different thresholds.
   - Useful for understanding the balance between the true positive rate and the positive predictive value.

5. **ROC Curve for the Best Model (Post Grid Search)**
   - Visualizes the ROC curve for the best model obtained from grid search optimization.
   - Indicates the model's effectiveness in classifying positive and negative cases.

### Insights

- The visualizations show that the Logistic Regression model has high accuracy, with a significant distinction between positive and negative cases.
- The ROC score of 0.94 for the best model indicates a strong predictive performance.
- The visualizations assist in comprehensively understanding the model's strengths and areas for improvement.

## Summary

- These visualizations form a crucial part of understanding and interpreting the behavior and performance of the machine learning models.
- Similar approaches can be replicated for other models to gain insights into their performance.

---
