# 📈 Sales Prediction using Python

A machine learning project that predicts product **Sales** based on advertising expenditure across **TV**, **Radio**, and **Newspaper** channels using **Linear Regression**.

This project was built as **Task 2** of my Data Science Internship at **CodeAlpha**.

---

## 📌 Project Overview

Sales prediction is a common business problem — companies want to know how much they should spend on different advertising channels to maximize sales. This project analyzes the relationship between advertising spend and sales, builds a regression model to predict sales, and visualizes how each channel individually impacts predicted sales.

---

## 🎯 Objectives

- Explore and clean the advertising dataset
- Visualize relationships between ad spend (TV, Radio, Newspaper) and Sales
- Build and evaluate a Linear Regression model
- Compare model performance with and without feature scaling
- Create a reusable prediction function for new advertising spend values
- Visualize how varying each channel's spend impacts predicted sales

---

## 🗂️ Dataset

The project uses the **Advertising dataset**, which contains advertising spend (in thousands of dollars) across three media channels along with the resulting product sales.

| Column      | Description                          |
|-------------|---------------------------------------|
| TV          | Advertising spend on TV                |
| Radio       | Advertising spend on Radio             |
| Newspaper   | Advertising spend on Newspaper         |
| Sales       | Product sales (target variable)        |

---

## 🛠️ Tech Stack

- **Python**
- **Pandas** – data loading and manipulation
- **NumPy** – numerical operations
- **Matplotlib & Seaborn** – data visualization
- **Scikit-learn** – model building, scaling, and evaluation

---

## 🔍 Project Workflow

1. **Data Loading & Cleaning**
   - Loaded the dataset and removed the redundant index column
   - Checked for missing values and reviewed descriptive statistics

2. **Exploratory Data Analysis (EDA)**
   - Visualized TV, Radio, and Newspaper spend against Sales using regression plots

3. **Model Building**
   - Split data into training (80%) and testing (20%) sets
   - Trained a **Linear Regression** model on the raw features
   - Evaluated using **Mean Squared Error (MSE)** and **R² Score**

4. **Feature Scaling**
   - Applied `StandardScaler` to standardize the features
   - Retrained the model on scaled data and compared performance

5. **Prediction**
   - Built a reusable `predict_sales()` function to predict sales for any given ad spend combination
   - Predicted sales for sample/hypothetical advertising budgets

6. **Impact Analysis**
   - Varied TV, Radio, and Newspaper spend individually (holding others constant)
   - Visualized how predicted sales change with each channel's spend

---

## 📊 Results

The Linear Regression model shows a strong relationship between advertising spend and sales, with **TV** and **Radio** having the strongest positive impact on sales, while **Newspaper** spend shows a comparatively weaker effect. Feature scaling did not significantly change model performance (as expected for linear regression) but made the coefficients more directly comparable across features.

---

## 🖼️ Screenshots

### 📊 Ad Spend vs Sales (Regression Plots)
![Ad Spend vs Sales](https://github.com/SugamSagar-DS458/CodeAlphaInternship-Project/blob/main/Task2-SalesPricePrediction/Screenshot%202026-08-28%20191508.png)

### 📈 Predicted Sales vs TV Ad Spend
![TV Spend Impact](https://github.com/SugamSagar-DS458/CodeAlphaInternship-Project/blob/main/Task2-SalesPricePrediction/Screenshot%202026-08-28%20191330.png)

### 📈 Predicted Sales vs Radio Ad Spend
![Radio Spend Impact](https://github.com/SugamSagar-DS458/CodeAlphaInternship-Project/blob/main/Task2-SalesPricePrediction/Screenshot%202026-08-28%20191349.png)

### 📈 Predicted Sales vs Newspaper Ad Spend
![Newspaper Spend Impact](https://github.com/SugamSagar-DS458/CodeAlphaInternship-Project/blob/main/Task2-SalesPricePrediction/Screenshot%202026-08-28%20191402.png)

---

## 🚀 How to Run

1. **Clone the repository**
   ```bash
   git clone https://github.com/<your-username>/<repo-name>.git
   cd <repo-name>
   ```

2. **Install the required dependencies**
   ```bash
   pip install pandas numpy matplotlib seaborn scikit-learn jupyter
   ```

3. **Run the notebook**
   ```bash
   jupyter notebook SalesPrediction.ipynb
   ```

> Make sure the `Advertising.csv` dataset is placed in the same directory as the notebook, or update the file path in the first cell accordingly.

---

## 📁 Repository Structure

```
├── SalesPrediction.ipynb   # Main Jupyter notebook with full analysis
├── Advertising.csv         # Dataset (add this file to the repo)
├── screenshots/            # Output screenshots used in this README
│   ├── adspend_vs_sales.png
│   ├── tv_spend_impact.png
│   ├── radio_spend_impact.png
│   └── newspaper_spend_impact.png
└── README.md               # Project documentation
```

---

## 🏢 About the Internship

This project was completed as part of the **Data Science Internship at CodeAlpha**, where the goal was to apply machine learning techniques to solve real-world business problems using Python.

---

## 🙌 Acknowledgements

- **CodeAlpha** for the internship opportunity and project guidance
- The Advertising dataset, a widely used dataset for regression practice

---
