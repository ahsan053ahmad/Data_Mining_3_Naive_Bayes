# Data_Mining_3_Naive_Bayes

This repository contains an R Markdown assignment focused on training, validating, and evaluating a Naïve Bayes classification model. The goal was to develop a probabilistic classifier using Bayesian inference and evaluate its performance using cross-validation.

---

### Business Problem

Probabilistic models like Naïve Bayes are widely used for classification tasks such as spam detection, sentiment analysis, and medical diagnosis. Their simplicity, efficiency, and effectiveness—especially on high-dimensional data—make them ideal for early-stage modeling and benchmarking.

This project involved using a preprocessed dataset with labeled outcomes to predict class membership. The assignment emphasized understanding the theoretical basis of Naïve Bayes and implementing it with rigorous cross-validation to evaluate model performance and generalizability.

---

### Project Objective

The key objectives of the assignment were:

- To apply a Naïve Bayes classifier to a structured dataset
- To perform **10-fold cross-validation** to estimate model performance
- To assess the classifier using metrics such as **accuracy**, **precision**, and **recall**
- To compare model performance across cross-validation folds and test set results
- To interpret how prior and likelihood assumptions affect predictive outcomes

---

### Solution

The assignment workflow was broken down into the following stages:

- **Data Preparation**:
  - Cleaned and factorized categorical variables
  - Checked class distributions for training/test splits
- **Model Training**:
  - Used the `naiveBayes()` function from the `e1071` package
  - Trained the model using 10-fold cross-validation
- **Evaluation**:
  - Collected fold-wise performance metrics
  - Generated a confusion matrix and calculated precision/recall on the test set
- **Comparison**:
  - Evaluated cross-validation metrics vs. holdout test performance
  - Discussed the strengths and weaknesses of the Naïve Bayes assumptions

---

### Business Value

While this assignment was academic, the methodology reflects common real-world use cases:

- **Baseline Benchmarking**: Naïve Bayes serves as a fast and interpretable first-pass model
- **Text and Categorical Data**: Performs well in NLP tasks and categorical-heavy datasets
- **Explainability**: Probabilistic predictions and conditional likelihoods are easy to communicate
- **Speed and Efficiency**: Ideal for large-scale or real-time applications

---

### Challenges Encountered

- **Assumption Sensitivity**: Naïve Bayes assumes independence between features, which can limit its real-world performance
- **Cross-Validation**: Manual implementation required careful fold management and averaging
- **Precision vs. Recall**: Balancing false positives and false negatives was crucial for evaluation

---
