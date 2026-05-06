# Food-Nutrition-Data-Analysis-Classification-Model
# Nutritional Data Classification using Machine Learning

Machine learning pipeline for **multi-class classification** of food health ratings (Nutri-Score A–E) using the Open Food Facts dataset containing **350,000+ food products and 150+ features**. This project explores large-scale nutritional data preprocessing, classification modeling, dimensionality reduction, and feature importance analysis to better understand the factors driving food health scores.

---

## Project Overview

This project analyzes nutritional data from the Open Food Facts database and builds predictive models capable of classifying food products into Nutri-Score categories based on nutritional composition.

The workflow includes:

* Large-scale data preprocessing and cleaning
* Missing value handling and feature selection
* Exploratory data analysis (EDA)
* Multi-class classification modeling
* Principal Component Analysis (PCA)
* Model evaluation and error analysis
* Feature importance analysis

---

## Dataset

**Source:**

### Dataset Size

* 350,000+ records
* 150+ features
* Nutritional, categorical, and metadata attributes

### Key Features Used

* `energy_100g`
* `fat_100g`
* `saturated-fat_100g`
* `carbohydrates_100g`
* `sugars_100g`
* `proteins_100g`
* `fiber_100g`
* `salt_100g`

### Target Variable

* `nutrition_grade_fr`

  * Nutri-Score classifications:

    * A
    * B
    * C
    * D
    * E

---

## Machine Learning Workflow

### Data Processing

* Selected relevant nutritional features
* Removed and analyzed missing values
* Compared dropping null rows vs imputation strategies
* Encoded categorical target labels

### Modeling

Implemented and evaluated:

* Logistic Regression
* Scaled Logistic Regression
* Random Forest Classifier

### Dimensionality Reduction

Applied:

* Principal Component Analysis (PCA)

to analyze feature relationships and compare model performance against baseline feature sets.

### Model Evaluation

Used:

* Accuracy score
* Confusion matrix
* Classification report
* Error analysis

### Feature Importance Analysis

Identified the strongest contributors to Nutri-Score predictions, including:

* Salt
* Saturated fat
* Sugar

---

## Results

| Model                      | Accuracy |
| -------------------------- | -------- |
| Logistic Regression        | ~53%     |
| Scaled Logistic Regression | ~62%     |
| Random Forest Classifier   | ~94%     |

### Key Findings

* Feature scaling significantly improved Logistic Regression performance.
* Random Forest produced the strongest classification accuracy.
* The model primarily confused neighboring Nutri-Score classes (e.g., B vs C, C vs D), while rarely confusing extreme classes (A vs E).
* Salt, saturated fat, and sugar were identified as the most influential nutritional predictors.

---

# View the Notebook

## GitHub Notebook

Recruiters and reviewers can access the full notebook here:

👉 https://github.com/neysap/Food-Nutrition-Data-Analysis-Classification-Model/blob/main/World_Food_Facts.ipynb

---

## Open Directly in Google Colab

To run the notebook interactively in Google Colab:

1. Open the notebook link above
2. Click the **“Open in Colab”** button at the top of the notebook
 <img width="150" height="41" alt="image" src="https://github.com/user-attachments/assets/f35997c7-0454-48d3-a6c5-7479133a8c83" />


---

## Technologies Used

* Python
* Pandas
* NumPy
* Scikit-learn
* Matplotlib
* Google Colab
* Jupyter Notebook

---

## Skills Demonstrated

* Machine Learning
* Data Cleaning & Preprocessing
* Classification Modeling
* Feature Engineering
* Principal Component Analysis (PCA)
* Random Forest Classification
* Model Evaluation & Error Analysis
* Data Visualization
* Large-Scale Data Analysis

---

## Author

**Neysa Porter**
University of Pennsylvania — Master of Computer and Information Technology (MCIT)
Technology, Data, and Machine Learning Enthusiast
