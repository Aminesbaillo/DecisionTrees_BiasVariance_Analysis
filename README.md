
# Decision Trees: Bias-Variance Analysis & Rule Extraction

Welcome to the DecisionTrees_BiasVariance_Analysis repository! This project demonstrates how to build, evaluate, and interpret a Decision Tree model for classification tasks, with a focus on understanding the bias-variance tradeoff and extracting transparent decision rules.

## Requirements

- Python 3.7+
- pandas for data manipulation
- NumPy for numerical operations
- scikit-learn for machine learning models
- matplotlib and seaborn for data visualization




## Installation

If you don’t have any of these libraries installed, you can install them via:

```bash
pip install pandas numpy scikit-learn matplotlib seaborn
```
    
## Documentation

[Theoretical Background: Decision Trees](https://linktodocumentation)

A Decision Tree is a supervised learning algorithm used for both classification and regression tasks. It works by repeatedly splitting the data into smaller subsets based on certain thresholds of feature values, forming a tree-like structure of decision paths. Key concepts include:

#### **Impurity Measures:**

1. **Gini Index:** Measures how often a randomly chosen element would be incorrectly labeled if it were randomly labeled according to class distribution.
Entropy: Quantifies the uncertainty or disorder in the dataset.

2. **Splitting Criteria:**
Decision Trees try to find the optimal feature and threshold that result in the most “pure” subsets. Lower impurity indicates a better split.

3. **Depth & Pruning:**
Increasing tree depth can cause the model to overfit (high variance). Pruning or limiting the depth helps reduce complexity and avoid overfitting.


#### **How We Applied It Here ?**
1. **Data Exploration:**

Loaded the classic Iris dataset and examined distributions and correlations to understand relationships between features.

2. **Model Training:**

Trained Decision Trees using two different criteria (Gini and Entropy).
Adjusted hyperparameters (tree depth) to analyze the bias-variance tradeoff.

3. **Evaluation:**

Compared training vs. testing accuracy to illustrate underfitting vs. overfitting.
Created visual plots to highlight how tree depth impacts performance.

3. **Interpretation:**

Used the export_text function to generate human-readable decision rules.
Visualized the final tree to showcase its splits and thresholds.

#### **Definitions of Key Terms**
* **Bias:** The difference between the predicted values and the true values on average. A high-bias model is typically too simple and underfits the data.
* **Variance:** How much the model’s predictions change when training on different subsets of the data. A high-variance model overfits the data and doesn’t generalize well.
* **Overfitting:** When a model learns not just the underlying relationships but also the noise in the training data, causing poor performance on unseen data.
* **Underfitting:** When a model is too simple and fails to capture the underlying pattern in the data, resulting in high bias and low accuracy.
* **Impurity:** A measure of how mixed the classes are within a subset. Lower impurity generally means a better split.
* **Threshold:** A cutoff value at which data is split into two groups based on a selected feature.


## Usage

1. **Clone** or **download** this repo.
2. **Install** the requirements listed above.
3. **Open** the Jupyter Notebook (.ipynb) to view and run the code cells step-by-step.


Feel free to explore and modify the notebook to suit your own classification tasks. If you have any questions or feedback, please open an issue or submit a pull request. Enjoy learning about Decision Trees!
