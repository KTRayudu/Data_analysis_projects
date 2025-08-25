# Data_analysis_projects


# Data Analysis Portfolio

Welcome to my data analysis portfolio. This repository contains a collection of projects demonstrating my skills in data cleaning, exploratory data analysis (EDA), data visualization, and statistical analysis using Python (Pandas, Matplotlib, Seaborn) and Excel. Each project is contained within its own Jupyter Notebook.

## Table of Contents
1.  [Project 1: Sleep Health and Lifestyle Analysis](#project-1-sleep-health-and-lifestyle-analysis)
2.  [Project 2: Exploratory Data Analysis of Loan Applications](#project-2-exploratory-data-analysis-of-loan-applications)
3.  [Project 3: Descriptive Statistics on Employee Wages](#project-3-descriptive-statistics-on-employee-wages)
4.  [Project 4: Superstore Sales Dashboard Analysis](#project-4-superstore-sales-dashboard-analysis)
5.  [Project 5: Customer Behavior and Financial Analysis](#project-5-customer-behavior-and-financial-analysis)
6.  [Project 6: Movie Industry Financials EDA](#project-6-movie-industry-financials-eda)
7.  [Project 7: Sleep Disorder Classification Prep](#project-7-sleep-disorder-classification-prep)

---

### Project 1: Sleep Health and Lifestyle Analysis
* **File:** [`Project_1_Sleep_Health_Analysis.ipynb`](./Sleep_Health_Analysis.ipynb)
* **Skills:** Data Cleaning, Data Visualization (Matplotlib, Seaborn), Binary Classification, Health Data Analysis

#### **Objective**
This project analyzes the "Sleep Health and Lifestyle Dataset" to understand how various lifestyle factors (e.g., stress, physical activity) influence sleep quality and the presence of sleep disorders. The goal was to clean the data, identify key trends, and present a data-driven narrative through visualizations, making it highly relevant for public health data analysis.

#### **Methodology**
* **Data Cleaning:** Loaded the dataset using pandas and handled over 200 missing values in the `Sleep Disorder` column by imputing them with 'No Sleep Disorder'.
* **Feature Engineering:** Transformed the multi-class `Sleep Disorder` column into a binary target variable (`has_disorder`) to simplify the analysis.
* **Visualization & EDA:** Created scatter plots and box plots with seaborn to visualize relationships between `Stress Level`, `Sleep Duration`, and the presence of a sleep disorder.

#### **Key Findings**
The analysis revealed a strong correlation between higher stress levels and shorter sleep durations, which in turn was associated with a higher incidence of a diagnosed sleep disorder.

---

### Project 2: Exploratory Data Analysis of Loan Applications
* **File:** [`Project_2_Loan_Application_EDA.ipynb`](./Loan_Application_EDA.ipynb)
* **Skills:** Data Cleaning, Exploratory Data Analysis (EDA), Missing Value Imputation, Outlier Detection

#### **Objective**
To perform a comprehensive EDA on a loan application dataset to understand underlying patterns, clean the data for future machine learning modeling, and identify key variables that might influence loan approval status.

#### **Methodology**
* **Data Cleaning:** Handled missing values across multiple columns using mode imputation for categorical features (`Gender`, `Dependents`) and dropping rows for key numerical columns (`LoanAmount`, `Credit_History`).
* **EDA & Visualization:** Separated features into categorical and continuous types, generated descriptive statistics, and used box plots to identify outliers in financial columns.

#### **Key Findings**
The EDA produced a clean dataset ready for predictive modeling. The analysis revealed that a high percentage of applicants had a strong credit history, suggesting it as a critical predictive factor.

---

### Project 3: Descriptive Statistics on Employee Wages
* **File:** [`Project_3_Employee_Wage_Statistics.ipynb`](./Employee_Wage_Statistics.ipynb)
* **Skills:** Data Cleaning, Descriptive Statistics, Data Storytelling, Segmented Analysis

#### **Objective**
This project analyzes a dataset of employee wages for a fictitious tech company to derive insights into its compensation structure and demographic distribution, with the goal of informing HR policy.

#### **Methodology**
* **Data Preparation:** Cleaned the `Salary` column by removing non-numeric characters (`$`, `,`) and converting it to a float type. Engineered a `Start_Year` column from the `Start_date`.
* **Segmented Analysis:** Used `pd.crosstab` to analyze gender distribution across positions and visualized the results with a stacked bar chart. Examined salary distribution with a histogram.

#### **Key Findings**
Uncovered a significant gender imbalance in senior and management roles. The salary distribution was heavily right-skewed, with most employees in lower-paying production roles.

---

### Project 4: Superstore Sales Dashboard Analysis
* **File:** [`Project_4_Superstore_Sales_Dashboard.ipynb`](./Superstore_Sales_Dashboard.ipynb)
* **Skills:** Business Intelligence, Data Interpretation, KPI Analysis, Excel

#### **Objective**
To analyze a Power BI dashboard for a superstore to identify key business insights and provide strategic recommendations. This project demonstrates the ability to interpret data visualizations and translate them into actionable business intelligence.

#### **Methodology**
* Reviewed key performance indicators (KPIs) including total sales, profit, and order quantity.
* Analyzed sales performance over time, by product category, and by customer segment.
* Interpreted a map visualization to understand regional sales distribution.

#### **Key Findings**
Identified the "West" region as the top performer in sales. Found that "Phones" and "Chairs" were the most profitable sub-categories. Recommended targeted marketing for the "Consumer" segment, which had the highest sales.

---

### Project 5: Customer Behavior and Financial Analysis
* **File:** [`Project_5_Customer_Behavior_Analysis.ipynb`](./Customer_Behavior_Analysis.ipynb)
* **Skills:** Data Cleaning, Feature Engineering, Exploratory Data Analysis (EDA)

#### **Objective**
To perform an initial exploration of a dataset containing customer demographics and financial information. The focus was on data cleaning and preparing the data for more advanced analysis.

#### **Methodology**
* **Data Cleaning:** Assessed and handled missing values in multiple columns. Dropped rows where key financial data (`TotalCharges`) was missing.
* **Feature Engineering:** Converted the `TotalCharges` column from an object to a numeric type, handling errors and inconsistencies.
* **Initial EDA:** Generated descriptive statistics to get a baseline understanding of the numerical data distribution.

#### **Key Findings**
The initial data cleaning process successfully prepared the dataset for analysis. It was noted that `TotalCharges` required significant cleaning, and 11 out of 7043 records were dropped due to missing values.

---

### Project 6: Movie Industry Financials EDA
* **File:** [`Project_6_Movie_Industry_Financials.ipynb`](./Movie_Industry_Financials.ipynb)
* **Skills:** Data Cleaning (Type Conversion, String Manipulation), Exploratory Data Analysis

#### **Objective**
To clean and explore a dataset of movie financials, including production budgets, and domestic and worldwide gross revenues. The project focused on preparing the data for an analysis of profitability and trends in the film industry.

#### **Methodology**
* **Data Cleaning:** Performed extensive cleaning on financial columns by removing non-numeric characters (`$`, `,`) and converting them to numeric types for calculation.
* **Feature Exploration:** Conducted a `value_counts()` analysis on categorical columns like `distributor` and `genre` to understand the data distribution.

#### **Key Findings**
The data was successfully cleaned and transformed, making it ready for quantitative analysis. The initial exploration showed a wide variety of distributors and genres, with a heavy concentration in a few major categories.

---

### Project 7: Sleep Disorder Classification Prep
* **File:** [`Project_7_Sleep_Disorder_Classification_Prep.ipynb`](./Sleep_Disorder_Classification_Prep.ipynb)
* **Skills:** Data Preparation, Feature Scaling, Model Preparation (Scikit-learn)

#### **Objective**
This project serves as a precursor to machine learning modeling. The goal was to take the Sleep Health dataset, clean it, and prepare it for a classification task by encoding categorical variables and scaling numerical features.

#### **Methodology**
* **Data Loading & Initial Cleaning:** Loaded the dataset and performed an initial check for missing values and data types.
* **Feature Encoding:** Prepared for machine learning by separating features (`X`) from the target variable (`y`, Sleep Disorder). (Note: The notebook sets up the process, with the actual encoding and scaling steps to follow).

#### **Key Findings**
This notebook establishes the foundational data preparation steps required before training a classification model, such as identifying categorical and numerical features and separating the dataset into features and a target.
