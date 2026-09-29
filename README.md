# CDC Diabetes Health Indicators: Machine Learning Coursework

Exploratory data analysis, data visualisation, and comparative machine learning classification using the CDC Diabetes Health Indicators dataset.

## Project Overview

This project explores the CDC Diabetes Health Indicators dataset through exploratory data analysis (EDA), data visualisation, and a comparative evaluation of five machine learning classification models.

## Research Question

How do Logistic Regression, Decision Tree, Random Forest, Gaussian Naive Bayes, and Linear SVM compare in terms of accuracy, precision, recall, and F1-score when classifying the positive class in the CDC Diabetes Health Indicators dataset?

## Objectives

* Understand the structure and characteristics of the dataset.
* Explore the distribution of the target variable and health indicators.
* Visualise patterns and associations within the data.
* Train and evaluate five machine learning classification models.
* Compare model performance using accuracy, positive-class precision, recall, and F1-score.
* Discuss class imbalance and methodological limitations.

## Dataset

The dataset contains 253,680 records and 22 columns: 21 input features and one target variable, `Diabetes_binary`.

The target variable is defined as:

* `0`: No diabetes
* `1`: Prediabetes or diabetes

The positive class represents the combined prediabetes-or-diabetes category provided by the dataset. It should not be interpreted as confirmed diabetes alone.

The target distribution is imbalanced: approximately 86.1% of records belong to class 0 and 13.9% to class 1.

## Project Workflow

1. Review relevant research literature.
2. Inspect the dataset structure and data quality.
3. Perform exploratory data analysis.
4. Create visualisations of the target distribution and selected health indicators.
5. Prepare the data for classification.
6. Split the data into training and testing sets using stratified sampling.
7. Train five classification models.
8. Compare their performance on a common test set.
9. Interpret the findings and document limitations.

## Machine Learning Models

1. Logistic Regression
2. Decision Tree
3. Random Forest
4. Gaussian Naive Bayes
5. Linear Support Vector Machine (Linear SVM)

Feature scaling is used for Logistic Regression and Linear SVM in the current comparison.

## Evaluation Metrics

* **Accuracy:** Proportion of all predictions that are correct.
* **Positive-class precision:** Proportion of predicted positive cases that are actually positive.
* **Positive-class recall:** Proportion of actual positive cases identified by the model.
* **Positive-class F1-score:** Harmonic mean of positive-class precision and recall.

Because the dataset is imbalanced, accuracy is interpreted alongside positive-class precision, recall, and F1-score.

## Preliminary Results

In the current test-set comparison:

* Logistic Regression achieved the highest accuracy, approximately 86.2%.
* Linear SVM achieved the highest positive-class recall, approximately 76.9%, and F1-score, approximately 0.440.
* Gaussian Naive Bayes achieved a positive-class recall of approximately 56.4% and F1-score of approximately 0.408.

These findings illustrate trade-offs between overall accuracy and identification of the positive class. They apply to the current experimental setup and do not establish clinical suitability.

## Tools and Technologies

* Python
* Google Colab
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn
* GitHub

## Project Status

In progress. Initial exploratory data analysis, visualisation, and the five-model comparison have been completed. Further review of the methodology, evaluation, limitations, and documentation remains.

## Limitations and Disclaimer

This analysis identifies statistical patterns and evaluates classification performance within the selected dataset and experimental setup. Observed associations do not establish causation.

Results depend on the dataset, target definition, data preparation, model settings, and evaluation procedure. Further validation and methodological review are needed before drawing broader conclusions.

This is an academic machine learning project, not a clinical diagnostic tool. The models should not be used to diagnose diabetes or make individual medical decisions.
