## Data Quality Assessment & Preprocessing

## Project Overview

This project focuses on data preprocessing techniques applied to a student dataset. The main objective is to improve data quality and prepare the dataset for further analysis and machine learning tasks.

The preprocessing steps include handling missing values, detecting and treating outliers, normalizing numerical features, and applying dimensionality reduction using PCA.


## Dataset Source

Source: Student Performance Dataset
The dataset was obtained from Kaggle.

## Dataset Description

The dataset contains information about students, including:

* **age** → Student age
* **absences** → Number of school absences
and more

## Data Preprocessing Steps

### 1. Missing Values Handling

* Missing values were identified in the dataset
* Mean imputation was applied to fill missing values in numerical features 

### 2. Outlier Detection 

* Outliers were visualized using **boxplots**
* The **IQR method** was used to detect outliers
* Outliers were handled using:

  * **Capping (5th and 95th percentiles)**
* This approach reduces the effect of extreme values without removing data

### 3. Data Normalization

Two normalization techniques were applied:

* **Min-Max Scaling**

  * Scales values between 0 and 1

* **Z-score Normalization**

  * Transforms data to have mean = 0 and standard deviation = 1

### 4. Correlation Analysis

* A correlation heatmap was created to analyze relationships between features
* The correlation between **age** and **absences** was approximately **0.18**
* This indicates a weak relationship between the features

### 5. Principal Component Analysis (PCA)

* PCA was applied to reduce dimensionality
* The explained variance ratio was calculated
* Results showed that most of the variance is captured by the first principal component

Although the correlation between features is weak, PCA was applied for demonstration purposes.

## Tools and Libraries Used

* Python
* Pandas
* NumPy
* Matplotlib

