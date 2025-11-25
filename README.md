# EDA-for-Data-Science
This repository contains practical Exploratory Data Analysis (EDA) projects using Python to extract insights and patterns from real-world data.
# 📊 Exploratory Data Analysis using Python

This repository contains complete Exploratory Data Analysis (EDA) projects using Python and its powerful libraries.

![Python](https://img.shields.io/badge/Python-3.8+-blue?logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-purple?logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-Scientific%20Computing-blue?logo=numpy&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-Visualization-orange?logo=plotly&logoColor=white)
![Seaborn](https://img.shields.io/badge/Seaborn-Statistical%20Viz-teal)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange?logo=jupyter&logoColor=white)
![Scikit-learn](https://img.shields.io/badge/Scikit--learn-ML-yellow?logo=scikit-learn&logoColor=black)

## 🔹 Tools & Technologies
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook

## 🔹 Objectives
- Understand the data structure
- Handle missing values
- Analyze data distribution
- Find correlations between variables
- Visualize patterns and trends

## 🔹 Folder Structure
- `data/` → Raw and cleaned datasets
- `notebooks/` → EDA notebooks step-by-step
- `images/` → Saved plots and heatmaps
- `src/` → Python helper functions
- `reports/` → Final EDA summary

## 🔹 Types of Analysis Covered
✅ Univariate Analysis  
✅ Bivariate Analysis  
✅ Multivariate Analysis  
✅ Correlation Analysis  
✅ Outlier Detection  
✅ Data Cleaning  

## 🔹 Libraries & Modules Used

- **Python 3.x**
- **Pandas** – Data handling & manipulation
- **NumPy** – Numerical computing
- **Matplotlib** – Data visualization
- **Seaborn** – Statistical visualization
- **Scikit-learn** – Correlation & preprocessing
- **Jupyter Notebook** – Interactive analysis

---

# 01_data_overview.ipynb - Data Overview (copy-paste)

import pandas as pd
import numpy as np
from IPython.display import display, HTML

# 1. Load dataset
csv_path = "data/raw/dataset.csv"
df = pd.read_csv(csv_path)

# 2. Basic preview
print("Shape:", df.shape)
display(df.head(10))

# 3. Basic info & stats
print("\n--- Info ---")
display(df.info())
print("\n--- Describe ---")
display(df.describe(include='all').transpose())

# 4. Missing values
print("\nMissing values per column:")
display(df.isnull().sum())

# 5. Save a small HTML preview (optional)
preview_html = df.head(20).to_html(index=False)
with open("reports/dataset_preview.html", "w", encoding="utf-8") as f:
    f.write("<h3>Dataset Preview (first 20 rows)</h3>\n")
    f.write(preview_html)

print("\nSaved HTML preview: reports/dataset_preview.html")



## 📌 About Me
I am an AI & Data Science student working on real-world data analysis projects to improve my skills in EDA and Machine Learning.

