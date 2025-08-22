# L1-Regularized Logistic Regression: Sparsity and Geometry

This repo demonstrates how L1-regularized logistic regression affects sparsity in the weight vector and how it connects to the geometry of optimization constraints. It uses the Breast Cancer Wisconsin dataset to show the trade-off between model accuracy and simplicity when applying L1 regularization.

---

## What is L1-Regularized Logistic Regression?

Logistic regression with an L1 penalty adds a constraint that pushes many coefficients to zero.  
This results in:
- Sparsity - simpler, more interpretable models  
- Feature selection - irrelevant features get eliminated  
- Geometric intuition - feasible region shaped as a diamond (L1 ball), leading solutions to “stick” to corners  

---

## Features

- Data exploration and preprocessing (scaling, class balance handling)  
- Training with scikit-learn’s `LogisticRegression` (`penalty='l1'`)  
- Grid search for hyperparameter tuning (`C = 1/λ`)  
- Sparsity vs. regularization strength analysis  
