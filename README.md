# Simple Linear Regression from Scratch

This project implements a **Simple Linear Regression** model using **Gradient Descent** from scratch. It is designed to demonstrate the fundamental mathematics behind linear regression without relying on high-level machine learning libraries like `scikit-learn`.

## Table of Contents
- [Overview](#overview)
- [Mathematical Components](#mathematical-components)
- [Project Structure](#project-structure)
- [Installation and Usage](#installation-and-usage)
- [Results](#results)

## Overview
Linear regression is a linear approach to modeling the relationship between a scalar response and one or more explanatory variables. In this project, we implement a simple linear regression model where we predict a dependent variable $Y$ based on an independent variable $X$.

## Mathematical Components

### 1. Hypothesis Function
The model predicts the output using the following linear equation:
$$h_\theta(x) = \theta_0 + \theta_1x$$
In matrix form:
$$h_\theta(x) = X\theta$$

### 2. Cost Function (Mean Squared Error)
We use the Mean Squared Error (MSE) to measure the performance of our hypothesis:
$$J(\theta) = \frac{1}{2m} \sum_{i=1}^{m} (h_\theta(x^{(i)}) - y^{(i)})^2$$

### 3. Gradient Descent
To minimize the cost function, we update the parameters $\theta$ iteratively:
$$\theta_j := \theta_j - \alpha \frac{1}{m} \sum_{i=1}^{m} (h_\theta(x^{(i)}) - y^{(i)})x_j^{(i)}$$
where $\alpha$ is the learning rate.

## Project Structure
- `simple/Untitled2.ipynb`: The main Jupyter Notebook containing the implementation, training, and visualization.
- `README.md`: Project documentation.

## Installation and Usage

### Prerequisites
- Python 3.x
- NumPy
- Matplotlib
- Jupyter Notebook

### Running the Project
1. Open the terminal.
2. Navigate to the project directory:
   ```bash
   cd "regression lineare"
   ```
3. Launch Jupyter Notebook:
   ```bash
   jupyter notebook
   ```
4. Open `simple/Untitled2.ipynb` and run all cells.

## Results
The notebook provides:
- A scatter plot of the original data points.
- The fitted regression line after training.
- A cost history plot showing the convergence of Gradient Descent.
