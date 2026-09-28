# Unemployment Analysis with Python

## Project Overview

This project performs exploratory data analysis on unemployment data from India to investigate **regional and temporal patterns in unemployment rates**, with particular attention to the changes observed around the COVID-19 period.

The analysis uses Python, Pandas, Matplotlib, Seaborn, and Jupyter Notebook to clean the data, explore trends, create visualizations, and compare unemployment rates between Pre-COVID and Post-COVID periods.

## Objective

The main objectives of this project are:

* Clean and prepare the unemployment dataset.
* Analyze regional differences in unemployment.
* Study month-wise unemployment trends.
* Examine unemployment rates over time for selected regions.
* Identify the regions with the highest average unemployment rates.
* Analyze correlations between unemployment, employment, and labour participation.
* Compare Pre-COVID and Post-COVID unemployment rates.

## Dataset

The dataset contains information about unemployment across different regions of India.

Main columns include:

* `Region`
* `Date`
* `Frequency`
* `Estimated Unemployment Rate (%)`
* `Estimated Employed`
* `Estimated Labour Participation Rate (%)`
* `Area`

After cleaning, the dataset contained **740 observations** and **9 columns**, including the additional `Month` and `Period` analysis columns.

## Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Jupyter Notebook

## Data Cleaning

The following preprocessing steps were performed:

* Checked dataset shape and structure.
* Checked for missing values.
* Converted the `Date` column to datetime format.
* Converted numerical columns to appropriate numeric data types.
* Filled missing numerical values using the median.
* Filled missing categorical values using the mode.
* Removed rows where the date was unavailable.
* Created a `Month` column for monthly analysis.
* Created a `Period` column to distinguish Pre-COVID and Post-COVID observations.

After cleaning, the dataset contained no missing values.

## Exploratory Data Analysis

### 1. Region-wise Average Unemployment

The average unemployment rate was calculated for each region to identify regional differences in unemployment.

A bar chart was created to compare average unemployment rates across regions.

### 2. Month-wise Unemployment Trends

Monthly average unemployment rates were calculated to identify changes throughout the year.

The analysis showed particularly high average unemployment rates in:

* **April: 23.64%**
* **May: 16.65%**

Other months generally had lower average unemployment rates.

### 3. Regional Time-Series Analysis

A time-series line chart was created for:

* Punjab
* Maharashtra
* West Bengal

The chart shows how unemployment rates changed over time and demonstrates that unemployment patterns varied between regions.

### 4. Top 10 Regions

The top 10 regions with the highest average unemployment rates were identified using regional averages.

A bar chart was created to visualize these regions.

### 5. Correlation Analysis

A correlation heatmap was created for:

* Estimated Unemployment Rate
* Estimated Employed
* Estimated Labour Participation Rate

Important correlations observed in the dataset included:

| Variables                                      | Correlation |
| ---------------------------------------------- | ----------: |
| Unemployment Rate ↔ Estimated Employed         |       -0.22 |
| Unemployment Rate ↔ Labour Participation Rate  |       ~0.00 |
| Estimated Employed ↔ Labour Participation Rate |        0.01 |

The unemployment rate therefore showed a weak negative relationship with estimated employment, while the relationships involving labour participation were very weak.

> Correlation describes association between variables and does not establish causation.

## Pre-COVID vs Post-COVID Analysis

The data was divided into two periods using **March 2020** as the cutoff:

* Pre-COVID: before March 2020
* Post-COVID: March 2020 onward

### Results

| Period     | Average Unemployment Rate |
| ---------- | ------------------------: |
| Pre-COVID  |                     9.51% |
| Post-COVID |                    17.77% |

The Post-COVID period had an average unemployment rate approximately **8.26 percentage points higher** than the Pre-COVID period in this dataset.

This comparison shows a substantial change in unemployment rates between the two periods, although the analysis itself does not establish that COVID-19 was the sole cause of the change.

## Visualizations

The project includes:

* Region-wise average unemployment bar chart
* Month-wise unemployment trend line chart
* Regional time-series line chart
* Top 10 regions bar chart
* Correlation heatmap
* Pre-COVID vs Post-COVID comparison chart

## Project Workflow

```text
Load Dataset
      ↓
Data Cleaning
      ↓
Missing Value Handling
      ↓
Date & Data Type Conversion
      ↓
Exploratory Data Analysis
      ↓
Regional Analysis
      ↓
Monthly Trend Analysis
      ↓
Time-Series Analysis
      ↓
Correlation Analysis
      ↓
Pre-COVID vs Post-COVID Analysis
      ↓
Conclusions
```

## How to Run

1. Clone the repository.

```bash
git clone <your-repository-url>
```

2. Open Jupyter Notebook.

```bash
jupyter notebook
```

3. Open the unemployment analysis notebook.

4. Run the notebook cells sequentially.

## Project Structure

```text
Unemployment-Analysis/
│
├── Unemployment_Analysis.ipynb
├── unemployment_data.csv
├── README.md
└── requirements.txt
```

## Conclusion

The analysis demonstrates significant regional and temporal variation in unemployment rates across India.

The monthly analysis showed particularly high unemployment rates during April and May. Regional analysis also revealed differences between states and regions.

The Pre-COVID vs Post-COVID comparison showed an increase in the average unemployment rate from approximately **9.51% to 17.77%** in the dataset.

Overall, the project demonstrates how Python-based exploratory data analysis can be used to identify patterns, compare groups, and communicate insights through data visualization.
