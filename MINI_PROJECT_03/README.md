# Salary Prediction Using Linear Regression

## Project Overview

This project uses Linear Regression, a supervised machine learning algorithm, to predict employee salaries based on their years of work experience. The project includes data analysis, data preprocessing, outlier detection, model training, prediction, evaluation, and visualization using Python.

## Objective

* Perform initial data analysis.
* Handle missing values and duplicate records.
* Detect and remove outliers using the IQR method.
* Split the dataset into training and testing sets.
* Build a Linear Regression model.
* Predict salaries based on years of experience.
* Evaluate the model's performance using regression metrics.

## Dataset

**Dataset Name:** Salary_Data.csv

**Features:**

* YearsExperience: Number of years of work experience.
* Salary: Employee salary (target variable).

## Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Scikit-learn
* Linear Regression

## Project Workflow

### 1. Data Loading

Load the Salary_Data.csv dataset using Pandas and display the first five and last five rows.

### 2. Initial Data Analysis

Perform exploratory data analysis to understand the dataset.

* Check the number of rows and columns.
* Display dataset information and descriptive statistics.
* Identify numerical and categorical columns.
* Check missing values and duplicate records.

### 3. Data Preprocessing

Prepare the dataset for machine learning.

* Remove duplicate records.
* Fill missing numerical values using the median.
* Fill missing categorical values using the mode.

### 4. Outlier Detection Using IQR

Use the Interquartile Range (IQR) method to identify outliers in the Salary column.

**Formulas:**

* IQR = Q3 - Q1
* Lower Limit = Q1 - 1.5 × IQR
* Upper Limit = Q3 + 1.5 × IQR

Values below the lower limit or above the upper limit are identified as outliers. These records are removed to create a cleaned dataset.

### 5. Feature Selection

Select the independent and dependent variables.

* Independent Variable (X): YearsExperience
* Dependent Variable (y): Salary

The model uses years of experience to predict salary.

### 6. Train-Test Split

Split the dataset into two parts:

* Training Data: 80%
* Testing Data: 20%

The training data is used to train the model, while the testing data is used to evaluate its performance. A random state of 42 is used for reproducibility.

### 7. Model Training

Build and train a Linear Regression model using Scikit-learn.

The model learns the relationship between years of experience and salary.

### 8. Prediction

Use the trained model to predict salaries for the testing dataset.

### 9. Model Evaluation

Evaluate the model using the following regression metrics:

* **MAE (Mean Absolute Error):** Measures the average absolute difference between actual and predicted salaries.
* **MSE (Mean Squared Error):** Calculates the average squared difference between actual and predicted salaries.
* **RMSE (Root Mean Squared Error):** Measures prediction error in the same unit as salary.
* **R² Score:** Measures how much variation in salary is explained by the model.

### 10. Actual vs Predicted Values

Create a DataFrame containing the actual salaries and predicted salaries to compare the model's predictions with the actual values.

### 11. Data Visualization

Use Matplotlib to visualize the results.

* A scatter plot represents actual salary values.
* A regression line represents predicted salary values.
* The graph helps visualize the relationship between experience and salary.

## Expected Output

The program displays:

* Dataset information and descriptive statistics.
* Missing values and duplicate counts.
* IQR values and detected outliers.
* Cleaned dataset dimensions.
* Training and testing data sizes.
* Model coefficient and intercept.
* Predicted salary values.
* MAE, MSE, RMSE, and R² score.
* Actual vs predicted salary comparison.
* Linear Regression visualization.

## Conclusion

This project demonstrates how Linear Regression can be used to predict employee salaries based on years of experience. Data preprocessing and IQR-based outlier detection help prepare the dataset before model training. The evaluation metrics provide insights into prediction errors and model performance.

The project provides a basic machine learning workflow, from loading and cleaning data to training, prediction, evaluation, and visualization.
