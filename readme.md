# Lasso Regression – Machine Learning Practice

This repository contains my practice and notes for **Lasso Regression**, part of my daily **Machine Learning learning series** where I study and implement one algorithm at a time.

---

## What is Lasso Regression?

**Lasso Regression (Least Absolute Shrinkage and Selection Operator)** is a linear regression technique that uses **L1 regularization** to reduce overfitting and perform **automatic feature selection**.

It works by adding a penalty to the loss function which shrinks coefficients. Some coefficients may become **exactly zero**, effectively removing those features from the model.

---

## Mathematical Formula

Linear Regression minimizes:

\[
RSS = \sum (y - \hat{y})^2
\]

Lasso adds an **L1 penalty**:

\[
Loss = RSS + \lambda \sum |\beta|
\]

Where:

- **RSS** = Residual Sum of Squares  
- **β** = Model coefficients  
- **λ (lambda / alpha)** = Regularization strength  

---

## Key Idea

As **λ increases**:

- Coefficients **shrink**
- Some coefficients become **0**
- Irrelevant features are **removed from the model**

This helps create a **simpler and more interpretable model**.

---

## Lasso Path (Coefficient Shrinking)

The **Lasso Path graph** shows how coefficients change as regularization strength increases.

- Small λ → behaves like Linear Regression  
- Medium λ → coefficients shrink  
- Large λ → some coefficients become **0**

This demonstrates **feature selection in Lasso Regression**.

---

## Dataset

A **synthetic dataset** was generated using `sklearn.make_regression` with:

- 1200 rows
- 20 features
- 5 informative features
- Remaining features are noise

This helps clearly demonstrate how **Lasso removes irrelevant features**.

---

## Implementation Steps

1. Generate synthetic dataset  
2. Split dataset into training and testing sets  
3. Apply feature scaling using `StandardScaler`  
4. Train **Lasso Regression model**  
5. Analyze coefficients  
6. Visualize **Lasso coefficient path**

---

## Technologies Used

- Python
- NumPy
- Pandas
- Matplotlib
- Scikit-learn

---

## Learning Outcome

Through this practice I understood:

- L1 Regularization
- Overfitting and regularization
- Feature selection using Lasso
- Effect of lambda (α) on coefficients
- Lasso coefficient shrinking path

---

## Machine Learning Series

This project is part of my **daily Machine Learning practice series** where I learn and implement ML algorithms step by step.

Algorithms covered so far:

- Linear Regression
- Ridge Regression
- Lasso Regression

More algorithms coming soon.

---

## Connect With Me

If you are also learning Machine Learning, feel free to connect and follow my journey.

If you want the **notes or notebook used in this project**, reach out and I'll share them.

Happy Learning 🚀