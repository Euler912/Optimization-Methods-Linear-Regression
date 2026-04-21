This repository provides a comparative analysis of different optimization strategies applied to a Linear Regression task using the **California Housing dataset**. The project demonstrates how the choice of optimizer affects convergence speed, stability, and model performance.

## 🚀 Key Features

### 1. Robust Data Preprocessing
* **Outlier Removal**: Implementation of **Z-score** analysis to filter statistical noise.
* **Feature Engineering**: Selection of top predictors using **Mutual Information Regression**.
* **Normalization**: Full pipeline for feature scaling to ensure optimal gradient flow.

### 2. Multi-Optimizer Comparison
The project implements and benchmarks three distinct training approaches:
* **LBFGS**: A second-order quasi-Newton method that utilizes curvature information for extremely fast convergence.
* **SGD (Stochastic Gradient Descent)**: The standard first-order iterative method used in modern deep learning.
* **Manual Gradient Descent**: A "from-scratch" implementation built with **NumPy** to demonstrate the underlying mechanics of weight and bias updates.

### 3. Performance Analytics
* **Visualization**: Automated generation of loss curves for both training and validation sets.
* **Metric Evaluation**: Calculation of final Mean Squared Error (MSE) and gradient norms to verify convergence at critical points.

## 🛠 Tech Stack
* **Language**: Python
* **Deep Learning Framework**: PyTorch
* **Data Libraries**: NumPy, Pandas, Scikit-learn, SciPy
* **Visualization**: Matplotlib

## 📊 Summary of Results
The notebook illustrates that while **LBFGS** can converge in very few iterations, its stability depends heavily on the loss surface, whereas **SGD** provides a more gradual and robust descent. The manual implementation serves as a validation of the calculus logic behind the frameworks.
