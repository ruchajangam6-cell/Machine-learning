# Machine Learning Lab

This repository contains Python programs and practical work for the **Machine Learning Lab (IT3520)**. The experiments cover data preprocessing, exploratory data analysis, dimensionality reduction, supervised learning, regression, classification, clustering, and a basic artificial neural network.

## Experiments

| Experiment | Title / Topic | Main Concepts |
|---|---|---|
| 1 | Data Pre-processing on a Raw Dataset | Missing values, duplicates, outliers, normalization, standardization, encoding |
| 2 | Exploratory Data Analysis (EDA) | Summary statistics, visualizations, patterns, missing data, correlation |
| 3 | Principal Component Analysis (PCA) | Dimensionality reduction, standardization, explained variance, visualization |
| 4 | Linear Regression and Logistic Regression | Regression, classification, training/testing, model evaluation |
| 5 | Support Vector Machine (SVM) for Classification | Hyperplanes, support vectors, margins, kernels |
| 6 | Decision Tree and K-Nearest Neighbour (KNN) | Tree-based classification, distance metrics, scaling, classification metrics |
| 7 | Comparison of Regression Algorithms | Linear and polynomial regression, Decision Tree, Random Forest, SVR; MAE, MSE, R² |
| 8 | Comparison of Classification Algorithms | Logistic Regression, Decision Tree, Random Forest, SVM, KNN, Naive Bayes; precision, recall, accuracy |
| 9 | K-Means Clustering | Unsupervised learning, centroids, Euclidean distance, WCSS, Elbow Method |
| 10 | Single-Layer Artificial Neural Network (ANN) | Inputs, weights, bias, sigmoid activation, prediction, training |

## Technologies and Libraries

- Python 3
- Jupyter Notebook
- NumPy
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn

## Installation

1. Install Python 3 and Jupyter Notebook, or install Anaconda.
2. Clone or download this repository.
3. Open a terminal in the project folder.
4. Install the commonly used libraries:

```bash
pip install numpy pandas matplotlib seaborn scikit-learn jupyter
```

5. Start Jupyter Notebook:

```bash
jupyter notebook
```

6. Open an experiment notebook (`.ipynb`) and run the cells in order.

## Datasets

The practicals use datasets such as the Employee dataset, Titanic dataset, Iris dataset, and California Housing dataset. Some examples load datasets through Seaborn or Scikit-learn; other experiments may require a separate CSV file.

If an experiment uses a local CSV file, place that file in the same folder as the notebook or update the file path in the code. Follow the dataset source and instructions documented in the relevant experiment.

## Typical Machine Learning Workflow

1. Import the required libraries.
2. Load and inspect the dataset.
3. Clean and preprocess the data.
4. Separate input features and target labels, where applicable.
5. Split data into training and testing sets.
6. Train the selected algorithm.
7. Make predictions.
8. Evaluate results using appropriate metrics.
9. Visualize and interpret the results.
10. Write the conclusion for the experiment.

## Evaluation Metrics

Depending on the task, experiments may use:

- **Accuracy:** Overall proportion of correct predictions.
- **Precision:** Proportion of predicted positive cases that are correct.
- **Recall:** Proportion of actual positive cases correctly identified.
- **F1-score:** Harmonic mean of precision and recall.
- **MAE / MSE / RMSE:** Measures of regression prediction error.
- **R² score:** Measures how much variation in the target is explained by a regression model.
- **WCSS / Inertia:** Measures within-cluster variation in K-Means.

## Repository Structure

A suggested structure is:

```text
Machine-Learning-Lab/
├── README.md
├── Experiment-01-Data-Preprocessing.ipynb
├── Experiment-02-EDA.ipynb
├── Experiment-03-PCA.ipynb
├── Experiment-04-Linear-and-Logistic-Regression.ipynb
├── Experiment-05-SVM.ipynb
├── Experiment-06-Decision-Tree-and-KNN.ipynb
├── Experiment-07-Regression-Comparison.ipynb
├── Experiment-08-Classification-Comparison.ipynb
├── Experiment-09-KMeans-Clustering.ipynb
├── Experiment-10-Single-Layer-ANN.ipynb
└── datasets/
    └── Employee.csv
```

*The names above are suggestions. Use the actual filenames present in your repository.*

## Learning Outcomes

After completing these experiments, students should be able to:

- Prepare and explore datasets using Python.
- Apply preprocessing and feature scaling techniques.
- Build and compare common regression and classification models.
- Reduce feature dimensionality using PCA.
- Cluster unlabeled data using K-Means.
- Understand the basic learning process of a single-layer ANN.
- Evaluate models using suitable performance metrics.

## Notes

- Run notebook cells in order.
- Check that the required dataset files are available before running a notebook.
- Your output values may differ depending on the dataset, library versions, random seed, and train-test split.
- Include your own program outputs and observations when submitting practical work.

## Author

Add your name, department, college, and academic year here.
