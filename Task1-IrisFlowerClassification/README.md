# Iris Flower Classification

## Overview
This project builds a machine learning model to classify Iris flowers into their respective species based on sepal and petal measurements. The project involves data exploration, model training, evaluation, and visualization.

## Dataset
The dataset is loaded from an `Iris.csv` file. 
* **Total Entries:** 150 records.
* **Features:** `SepalLengthCm`, `SepalWidthCm`, `PetalLengthCm`, and `PetalWidthCm`.
* **Target:** `Species` (e.g., Iris-setosa, Iris-versicolor, Iris-virginica).
* **Data Quality:** The dataset is clean, with exactly 0 missing values across all columns.

## Methodology
1. **Data Preprocessing:** The `Id` and `Species` columns were dropped to isolate the feature variables (`X`), while the `Species` column was designated as the target variable (`y`).
2. **Train-Test Split:** The dataset was split into a training set of 105 samples (70%) and a testing set of 45 samples (30%) using a random state of 42.
3. **Model Training:** A Logistic Regression model was initialized with a maximum of 200 iterations (`max_iter=200`) and trained on the data. 
4. **Decision Boundary Visualization:** A secondary Logistic Regression model was trained exclusively on `PetalLengthCm` and `PetalWidthCm` to plot the 2D decision boundaries and visually map the classifications.

## Screenshots/Demo Video

### Logistic Regression Decision Boundaries (Petal Length vs. Petal Width
[Logistic Regression Decision Boundaries (Petal Length vs. Petal Width](https://github.com/SugamSagar-DS458/CodeAlphaInternship-Project/blob/main/Task1-IrisFlowerClassification/Screenshot%202026-08-28%20171424.png)

## Results
* **Accuracy:** The Logistic Regression model achieved a perfect accuracy score of **1.00 (100%)** on the testing set.

## Technologies Used
* **Python**.
* **Pandas**: For data manipulation and descriptive statistics.
* **Scikit-Learn**: For the train-test split, model training (`LogisticRegression`), and calculating model metrics (`accuracy_score`).
* **Matplotlib & Seaborn**: For creating the decision boundary contour maps and plotting the training points.
* **NumPy**: For generating mesh grids during visualization.

## Acknowledgements

Task completed as part of the **CodeAlpha Data Science Internship**.
