# Task-4-Classification-with-Logistic-Regression

1.Choose a binary classification dataset.

2.Train/test split and standardize features.

3.Fit a Logistic Regression model.

4.Evaluate with confusion matrix, precision, recall, ROC-AUC.

5.Tune threshold and explain sigmoid function.

---

# Objective:
Build a binary classifier using logistic regression.

---

# Tools: 
Scikit-learn, Pandas, Matplotlib

---

# Code Explanation 


1. Importing Libraries

Essential libraries like pandas, numpy, matplotlib, seaborn, and sklearn are imported.

These are used for data handling, model training, evaluation, and visualizations.



---

 2. Load Dataset

The dataset is read from your Google Drive path.

Columns like id and Unnamed: 32 (which are irrelevant) are dropped.



---

 3. Preprocessing

The diagnosis column (categorical) is converted to binary:

"M" (malignant) → 1

"B" (benign) → 0




---

 4. Feature and Target Split

X contains all feature columns.

y contains the binary target (diagnosis).



---

 5. Train/Test Split

The data is split into 80% training and 20% testing sets using train_test_split.



---

 6. Feature Standardization

Features are standardized using StandardScaler so that they all have mean 0 and standard deviation 1.

This is important for logistic regression to perform well.



---

 7. Train Logistic Regression Model

A logistic regression model is trained using the scaled training data.



---

 8. Predict Probabilities

The model outputs probabilities for class 1 (malignant).

Initially, a default threshold of 0.5 is used for classification.



---

 9. Evaluate Performance

Confusion Matrix: Shows TP, FP, TN, FN.

Precision: Fraction of correctly predicted positives.

Recall: Fraction of actual positives correctly predicted.

ROC-AUC Score: Measures overall classification performance.



---

 10. Visualize Confusion Matrix

A heatmap is plotted to clearly show the confusion matrix values for threshold 0.5.



---

 11. ROC Curve

The ROC curve (TPR vs FPR) is plotted to visualize model performance at various thresholds.

AUC (Area Under Curve) is printed.



---

 12. Threshold Tuning

A new threshold (e.g., 0.3) is tested to improve recall.

New predictions, precision, and recall are calculated.

A new confusion matrix heatmap is plotted for the tuned threshold.



---

 13. Sigmoid Function Explanation

Sigmoid function is explained:

It maps the linear output of logistic regression to a probability between 0 and 1.


A graph of the sigmoid function is plotted with reference lines at z=0 and p=0.5.



---

 14. Precision & Recall vs Threshold

Precision and recall scores are calculated across various thresholds.

A line plot shows how precision and recall change as the threshold is adjusted.

Helps visualize the trade-off and choose an optimal threshold.



---
