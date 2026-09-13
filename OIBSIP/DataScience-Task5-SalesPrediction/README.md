# 📊 Sales Prediction Using Machine Learning

<div align="center">

## Oasis Infobyte — Data Science Internship

### 📈 Task 5: Sales Prediction Using Machine Learning

**👨‍💻 Author:** Himanshu Chavda

![Python](https://img.shields.io/badge/Python-3.x-blue?logo=python)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-150458?logo=pandas)
![NumPy](https://img.shields.io/badge/NumPy-Numerical%20Computing-013243?logo=numpy)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-Machine%20Learning-F7931E?logo=scikit-learn)
![Matplotlib](https://img.shields.io/badge/Matplotlib-Visualization-11557C)
![Seaborn](https://img.shields.io/badge/Seaborn-Statistical%20Visualization-4C72B0)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-F37626?logo=jupyter)

</div>

---

## 📑 Table of Contents

* [Project Overview](#-project-overview)
* [Project Highlights](#-project-highlights)
* [Objective](#-objective)
* [Dataset Information](#-dataset-information)
* [Project Workflow](#-project-workflow)
* [Technologies Used](#️-technologies-used)
* [Exploratory Data Analysis](#-exploratory-data-analysis)
* [Machine Learning Models](#-machine-learning-models)
* [Model Evaluation](#-model-evaluation)
* [Residual Analysis](#-residual-analysis)
* [Feature Importance](#-feature-importance)
* [Project Structure](#-project-structure)
* [Output Files](#-output-files)
* [Project Visualizations](#-project-visualizations)
* [Results](#-results)
* [Key Insights](#-key-insights)
* [Future Improvements](#-future-improvements)
* [How to Run](#️-how-to-run)
* [License](#-license)
* [Author](#-author)
* [Internship](#-internship)

---

## 📌 Project Overview

This project develops a machine learning regression system to predict product sales based on advertising expenditure across three marketing channels:

* Television
* Radio
* Newspaper

The project follows an end-to-end Data Science workflow, including dataset inspection, data cleaning, exploratory data analysis, correlation analysis, machine learning model development, model evaluation, residual analysis, and feature importance analysis.

Two regression algorithms are trained and compared to identify the best-performing model for sales prediction.

---

## ✨ Project Highlights

* Dataset inspection and validation
* Missing-value analysis
* Duplicate-record analysis
* Descriptive statistical analysis
* Pairplot visualization
* TV, Radio, and Newspaper advertising analysis
* Advertising expenditure versus Sales scatter plots
* Correlation matrix and heatmap
* Linear Regression baseline model
* Random Forest Regression model
* Model comparison using MAE, RMSE, and R² Score
* Actual versus predicted sales analysis
* Residual analysis
* Linear Regression coefficient analysis
* Random Forest feature importance analysis
* Sample sales prediction
* CSV output generation
* Clean and documented Jupyter Notebook

---

## 🎯 Objective

The primary objective of this project is to build a supervised machine learning regression model that predicts product sales using advertising expenditure.

The project aims to:

* Understand the relationship between advertising expenditure and sales.
* Analyze the contribution of TV, Radio, and Newspaper advertising.
* Train and compare multiple regression models.
* Evaluate model performance using standard regression metrics.
* Identify the advertising channel with the strongest predictive contribution.
* Demonstrate sales prediction using a hypothetical advertising budget.

### Problem Type

**Supervised Learning — Regression**

### Input Features

* `TV`
* `Radio`
* `Newspaper`

### Target Variable

* `Sales`

---

## 📂 Dataset Information

### Dataset Name

**Advertising Dataset**

The dataset contains advertising expenditure and corresponding product sales information.

### Dataset Features

| Feature     | Description                                |
| ----------- | ------------------------------------------ |
| `TV`        | Advertising expenditure through television |
| `Radio`     | Advertising expenditure through radio      |
| `Newspaper` | Advertising expenditure through newspapers |
| `Sales`     | Product sales used as the target variable  |

The original dataset also contains an unnamed index column. This column is removed during data cleaning because it does not provide useful predictive information.

---

## 🔬 Project Workflow

```text
Load Dataset
     │
     ▼
Dataset Inspection
     │
     ▼
Data Cleaning
     │
     ▼
Remove Unnecessary Index Column
     │
     ▼
Missing Value Analysis
     │
     ▼
Duplicate Record Analysis
     │
     ▼
Descriptive Statistics
     │
     ▼
Exploratory Data Analysis
     │
     ▼
Pairplot Visualization
     │
     ▼
Advertising versus Sales Scatter Plots
     │
     ▼
Correlation Analysis
     │
     ▼
Correlation Heatmap
     │
     ▼
Feature and Target Selection
     │
     ▼
Train-Test Split
     │
     ▼
Linear Regression
     │
     ▼
Random Forest Regression
     │
     ▼
Model Evaluation
     │
     ▼
Model Comparison
     │
     ▼
Actual versus Predicted Analysis
     │
     ▼
Residual Analysis
     │
     ▼
Feature Importance Analysis
     │
     ▼
Sample Sales Prediction
     │
     ▼
Save Final Outputs
     │
     ▼
Conclusion
```

---

## 🛠️ Technologies Used

| Technology       | Purpose                              |
| ---------------- | ------------------------------------ |
| Python           | Programming language                 |
| Pandas           | Data loading, cleaning, and analysis |
| NumPy            | Numerical computation                |
| Matplotlib       | Data visualization                   |
| Seaborn          | Statistical visualization            |
| Scikit-Learn     | Machine learning model development   |
| Jupyter Notebook | Project development environment      |

---

## 📊 Exploratory Data Analysis

The notebook includes the following exploratory analysis:

* Dataset shape and structure
* Data types
* Missing-value inspection
* Duplicate-record inspection
* Descriptive statistics
* Pairplot of numerical variables
* TV advertising versus Sales scatter plot
* Radio advertising versus Sales scatter plot
* Newspaper advertising versus Sales scatter plot
* Correlation matrix
* Correlation heatmap

### Visualization Objectives

The visualizations are used to understand:

* Relationships between advertising expenditure and sales
* Positive or negative associations
* Possible outliers
* Differences between advertising channels
* The strength of linear relationships

Correlation is used as an exploratory measure and does not prove a causal relationship.

---

## 🤖 Machine Learning Models

Two regression models were implemented and evaluated.

### 1. Linear Regression

Linear Regression was used as the baseline regression model.

It learns a linear relationship between advertising expenditure and product sales.

The general form of the model is:

```text
Sales = β₀ + β₁(TV) + β₂(Radio) + β₃(Newspaper)
```

#### Advantages

* Simple and interpretable
* Easy to understand
* Provides feature coefficients
* Useful as a regression baseline

### 2. Random Forest Regressor

Random Forest Regressor is an ensemble machine learning algorithm that combines multiple decision trees to generate predictions.

It was used as an alternative model to evaluate whether nonlinear relationships could improve sales prediction.

#### Advantages

* Can model nonlinear relationships
* Handles feature interactions
* Provides feature importance scores
* Performs well on many structured datasets

---

## 📈 Model Evaluation

The models were evaluated using the following regression metrics:

| Metric   | Description                      | Preferred Value |
| -------- | -------------------------------- | --------------- |
| MAE      | Mean Absolute Error              | Lower           |
| RMSE     | Root Mean Squared Error          | Lower           |
| R² Score | Proportion of explained variance | Higher          |

### Mean Absolute Error

MAE measures the average absolute difference between actual and predicted sales values.

### Root Mean Squared Error

RMSE measures prediction error and gives greater importance to larger errors.

### R² Score

R² Score measures how much of the variation in the target variable is explained by the model.

The best-performing model is selected based on its performance on the unseen test dataset.

---

## 📉 Residual Analysis

Residuals represent the difference between actual and predicted sales values.

```text
Residual = Actual Sales − Predicted Sales
```

Residual analysis helps examine the quality of the regression model.

A well-behaved residual plot generally shows:

* Residuals distributed around zero
* No obvious systematic pattern
* No strong curve
* No clear funnel-shaped structure

The notebook includes:

* Residual scatter plot
* Residual distribution histogram
* Residual interpretation

---

## 🌟 Feature Importance

Feature importance analysis is performed using two approaches.

### Linear Regression Coefficients

Linear Regression coefficients help explain the estimated change in predicted Sales when one advertising feature increases by one unit while the other features remain constant.

### Random Forest Feature Importance

Random Forest feature importance scores indicate the relative predictive contribution of each advertising channel to the trained model.

The most important advertising channel is identified automatically in the notebook.

> Feature importance and correlation indicate predictive relationships. They should not be interpreted as proof of causal impact.

---

## 📁 Project Structure

```text
DataScience-Task5-SalesPrediction/
│
├── 📂 data/
│   └── advertising.csv
│
├── 📂 images/
│   ├── actual_vs_predicted_sales.png
│   ├── correlation_heatmap.png
│   ├── linear_regression_coefficients.png
│   ├── newspaper_vs_sales.png
│   ├── pairplot_relationships.png
│   ├── radio_vs_sales.png
│   ├── random_forest_feature_importance.png
│   ├── residual_distribution.png
│   └── tv_advertising_vs_sales.png
│
├── 📂 notebook/
│   └── sales_prediction.ipynb
│
├── 📂 outputs/
│   ├── actual_vs_predicted_sales.csv
│   ├── final_model_summary.csv
│   ├── linear_regression_coefficients.csv
│   ├── model_comparison.csv
│   ├── random_forest_feature_importance.csv
│   └── sample_sales_prediction.csv
│
└── README.md
```

---

## 📦 Output Files

The notebook exports the following files into the `outputs` directory:

| Output File                            | Description                                                   |
| -------------------------------------- | ------------------------------------------------------------- |
| `model_comparison.csv`                 | Performance comparison of Linear Regression and Random Forest |
| `linear_regression_coefficients.csv`   | Linear Regression coefficients for advertising channels       |
| `random_forest_feature_importance.csv` | Random Forest feature importance scores                       |
| `actual_vs_predicted_sales.csv`        | Actual sales, predicted sales, and residual values            |
| `final_model_summary.csv`              | Best model and final evaluation summary                       |
| `sample_sales_prediction.csv`          | Prediction for a hypothetical advertising budget              |

---

## 📷 Project Visualizations

The `images` folder contains visual outputs generated from the notebook.

### Pairplot

Shows pairwise relationships among:

* TV
* Radio
* Newspaper
* Sales

### Advertising versus Sales

Includes scatter plots for:

* TV advertising versus Sales
* Radio advertising versus Sales
* Newspaper advertising versus Sales

### Correlation Heatmap

Displays the correlation between the numerical variables in the dataset.

### Actual versus Predicted Sales

Compares actual sales values with predictions generated by the best-performing model.

### Residual Analysis

Includes:

* Residual scatter plot
* Residual distribution histogram

### Feature Importance

Includes:

* Linear Regression coefficient visualization
* Random Forest feature importance visualization

---

## 📈 Results

The project trains and compares Linear Regression and Random Forest Regression models using the same training and testing datasets.

The final model comparison includes:

* Mean Absolute Error
* Root Mean Squared Error
* R² Score

The best-performing model is selected automatically according to its test-set performance.

The project also identifies the advertising channel with the highest predictive importance using Random Forest feature importance.

> The exact model scores and best model name should be updated in this section after the final notebook execution.

---

## 💡 Key Insights

* Advertising expenditure can be used to predict product sales through supervised learning.
* TV, Radio, and Newspaper advertising have different relationships with Sales.
* Linear Regression provides an interpretable baseline model.
* Random Forest can capture nonlinear relationships and feature interactions.
* MAE and RMSE measure prediction error.
* R² Score measures the proportion of explained variance.
* Residual analysis helps identify possible prediction patterns and errors.
* Feature importance helps identify the advertising channel with the strongest predictive contribution.
* Predictive importance does not necessarily represent causal business impact.

---

## 🚀 Future Improvements

Possible future improvements include:

* Hyperparameter tuning using `GridSearchCV`
* K-fold cross-validation
* Additional regression algorithms
* Polynomial Regression
* Gradient Boosting Regression
* XGBoost Regression
* Outlier analysis
* Advertising budget optimization
* Return on Investment analysis
* Model deployment using Streamlit
* REST API development using Flask or FastAPI
* Model monitoring and retraining

---

## ▶️ How to Run

### 1. Clone the Repository

```bash
git clone YOUR_GITHUB_REPOSITORY_URL
```

### 2. Navigate to the Task Folder

```bash
cd DataScience-Task5-SalesPrediction
```

### 3. Install Required Libraries

```bash
pip install pandas numpy matplotlib seaborn scikit-learn jupyter
```

### 4. Launch Jupyter Notebook

```bash
jupyter notebook
```

### 5. Open the Notebook

```text
notebook/sales_prediction.ipynb
```

### 6. Run the Notebook

Run all notebook cells from top to bottom.

The notebook will:

* Load and clean the dataset.
* Perform exploratory data analysis.
* Train both regression models.
* Evaluate model performance.
* Generate visualizations.
* Perform residual analysis.
* Analyze feature importance.
* Generate a sample sales prediction.
* Save CSV output files in the `outputs` folder.

---

## 📄 License

This project was developed for educational purposes as part of the **Oasis Infobyte Data Science Internship Program**.

---

## 👨‍💻 Author

**Himanshu Chavda**

Data Science | Machine Learning | Artificial Intelligence | Data Analysis

* GitHub: `YOUR_GITHUB_PROFILE_URL`
* LinkedIn: `YOUR_LINKEDIN_PROFILE_URL`

---

## 📌 Internship

This project was completed as part of the **Oasis Infobyte Data Science Internship — Data Science Track**.

⭐ If you found this project useful, consider giving the repository a star.