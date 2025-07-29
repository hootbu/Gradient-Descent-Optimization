# Gradient Descent Optimization and Cost Function Visualization Project
###### Created by Emir Yorgun

## Overview

This project demonstrates an implementation of **gradient descent optimization** and **cost function visualization** applied to a noisy linear dataset. Utilizing Python with libraries such as **NumPy** and **Matplotlib**, the study follows a structured procedure to generate synthetic data, optimize parameters, and visualize results. The approach focusing on **mean squared error (MSE)** as the cost function and exploring the impact of **learning rate** and **iteration count** on convergence. This work showcases an effective application of **machine learning fundamentals** for linear regression analysis.

## Project Details

### Procedure and Implementation

1. **Data Generation**: A synthetic dataset with **100 data points** was created using **NumPy**. The underlying linear trend was defined as **y = 4x**, with **random noise** multiplied by a factor of **1.5** added to simulate real-world variability. The **x-values** were generated using `np.linspace(0, 10, 100)`, and corresponding **y-values** were calculated. A scatter plot was produced to visualize the **noisy linear trend**.
   
2. **Parameter Initialization**: Initial values for the **learning rate**, **number of iterations**, and **model parameters** were set to facilitate the **gradient descent algorithm**. These parameters were carefully chosen to ensure effective optimization.

3. **Gradient Descent Implementation**: 
   - A **compute_cost** function was developed to calculate the **mean squared error**, providing a measure of the model's accuracy.
   - A **gradient_descent** function was coded to iteratively adjust parameters, determining the **optimal weight (w)** for the linear model. The implementation successfully converged to an optimal solution for the dataset.

4. **Result Visualization**: 
   - The **optimal linear regression line** was plotted alongside the data points, offering a clear comparison.
   - A **cost history plot** was generated to illustrate the **convergence behavior** of the gradient descent algorithm over iterations, highlighting the reduction in error.
   - **Result Visualization Description**: The generated plot displays a scatter plot of the noisy dataset (blue dots) with **x-values** ranging from 0 to 10 and **y-values** reflecting the linear trend **y = 4x** plus added noise. The red line represents the fitted linear regression model, demonstrating how well the algorithm approximates the data. The visualization effectively highlights the relationship between the noisy data points and the optimized regression line, with the slope closely aligning with the true value of **4**.

5. **Discussion and Analysis**: 
   - The **learning rate** plays a critical role in optimization. A **high learning rate** may cause divergence, while a **low learning rate** can lead to slow convergence. An appropriate balance was selected for this project.
   - The **number of iterations** affects accuracy, with diminishing returns observed beyond a certain point. This suggests an optimal iteration count where further increases yield minimal improvement.

### Results
- The **gradient descent algorithm** successfully fitted a linear model, with the **optimal weight** closely aligning with the true value of **4**.
- The **cost history** demonstrated a steady decrease, confirming effective convergence.

## Acknowledgements

This project was inspired by academic resources and guidelines, providing a solid foundation for applying **gradient descent** and **visualization techniques** in machine learning.
