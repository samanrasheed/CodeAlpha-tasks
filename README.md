# Data Science Internship Projects

This repository contains the data science projects completed during my Data Science Internship. The projects cover machine learning, exploratory data analysis, data preprocessing, visualization, and statistical analysis using Python.

---

##  Projects

### 1. Iris Flower Classification

A machine learning classification project using the Iris dataset to predict the species of an iris flower based on its sepal and petal measurements.

####  Objective

The objective of this project is to build and evaluate machine learning models that can classify iris flowers into three species:

- Setosa
- Versicolor
- Virginica

####  Dataset

The Iris dataset is provided by Scikit-learn and contains:

- 150 observations
- 4 numerical features

Features:

- Sepal Length
- Sepal Width
- Petal Length
- Petal Width

Target:

- Iris Species

####  Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook

####  Project Workflow

1. Load the Iris dataset
2. Create a Pandas DataFrame
3. Perform exploratory data analysis
4. Check data types and missing values
5. Visualize feature relationships
6. Analyze feature distributions
7. Split data into training and testing sets
8. Apply feature scaling for KNN
9. Train machine learning models
10. Evaluate model performance
11. Compare the models using accuracy and confusion matrices

####  Machine Learning Models

Two classification algorithms were used:

- Logistic Regression
- K-Nearest Neighbors (KNN)

####  Results

| Model | Accuracy |
|-------|----------|
| Logistic Regression | 96.67% |
| K-Nearest Neighbors | 100% |

KNN achieved the highest accuracy on the evaluated test split, correctly classifying all 30 test observations.

Logistic Regression achieved approximately 96.67% accuracy, with one Versicolor sample classified as Virginica.

####  Key Insights

- Petal length and petal width were highly useful for distinguishing between species.
- Setosa was clearly separated from the other two species.
- Versicolor and Virginica showed some overlap.
- KNN performed slightly better than Logistic Regression on the evaluated test set.

####  Project File

`Iris-Flower-Classification/Iris_Flower_Classification.ipynb`

---

# 2. Unemployment Analysis with Python

An exploratory data analysis project focused on analyzing unemployment trends in different regions of India and understanding changes in unemployment before and after the COVID-19 period.

####  Objective

The objective of this project is to analyze unemployment patterns across Indian states and regions, identify temporal trends, and compare unemployment levels before and after COVID-19.

####  Dataset

The dataset contains unemployment-related information for different regions of India.

Main columns include:

- Region
- Date
- Frequency
- Estimated Unemployment Rate (%)
- Estimated Employed
- Estimated Labour Participation Rate (%)
- Area

Additional features were created during analysis:

- Month
- Period

####  Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook

####  Data Cleaning

The following preprocessing steps were performed:

- Checked for missing values
- Converted the Date column into datetime format
- Converted numerical columns into appropriate numeric data types
- Filled missing numerical values using median values
- Filled missing categorical values using the mode
- Removed rows with invalid dates
- Created Month and Period features
- Verified the final dataset for missing values

####  Exploratory Data Analysis

The following analyses were performed:

### Regional Unemployment Analysis

Calculated the average unemployment rate for each region and identified regions with higher unemployment rates.

### Monthly Unemployment Analysis

Calculated the average unemployment rate for each month to identify seasonal patterns.

April had the highest average unemployment rate at approximately 23.64%, followed by May at approximately 16.65%.

### Time-Series Analysis

Unemployment trends were visualized over time for selected regions, including:

- Punjab
- Maharashtra
- West Bengal

### Top 10 Regions

The top 10 regions with the highest average unemployment rates were identified and visualized.

### Correlation Analysis

A correlation matrix was created to analyze relationships between:

- Estimated Unemployment Rate
- Estimated Employed
- Labour Participation Rate

The unemployment rate showed a weak negative correlation with estimated employment, while the relationship with labour participation was close to zero.

### COVID-19 Analysis

The dataset was divided into:

- Pre-COVID
- Post-COVID

The average unemployment rates were:

| Period | Average Unemployment Rate |
|--------|---------------------------|
| Pre-COVID | 9.51% |
| Post-COVID | 17.77% |

The analysis shows an increase of approximately 8.26 percentage points in the average unemployment rate during the post-COVID period.

####  Key Insights

- Unemployment varied considerably across regions.
- April and May showed particularly high average unemployment rates.
- Different regions experienced different unemployment trends over time.
- The relationship between unemployment and estimated employment was weakly negative.
- The average unemployment rate was substantially higher in the post-COVID period.
- These results describe observed patterns and do not by themselves establish causation.

####  Project File

`Unemployment-Analysis/Unemployment_Analysis.ipynb`

---
