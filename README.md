# Applied Data Science

## Overview
This repository contains an applied data science project notebook focused on **Exploratory Data Analysis (EDA)**, **Data Preprocessing**, and **Visualization** using a financial/transactional dataset (`ADS_DATASET.csv`).

The primary goal of this project is to clean, transform, and visualize the data to extract insights related to transaction **amounts**, **modes**, and **categories**.

---

## Key Features & Analysis

The project notebook demonstrates several data processing and visualization techniques:

### Data Preprocessing & Feature Engineering
* **Data Inspection:** Initial loading and display of the dataset, which includes columns like `Date`, `Mode`, `Category`, `Subcategory`, and `Amount`.
* **Normalization & Scaling:**
    * **Z-score Normalization**.
    * **Min-Max Normalization** (scaling to a [0, 1] range).
    * **Decimal Scaling Normalization**.
* **Feature Selection:** An attempt was made to apply ANOVA F-value testing via `SelectKBest`, though this step was skipped as no explicit target variable was defined (`Amount` was excluded as a target in the original code snippet).

### Data Visualization
The notebook includes various charts to understand data distribution and relationships:
* **Bar Graph:** Visualizing the relationship between **Top Occurring Modes** (e.g., 'Cash', 'Saving Bank account 1', 'Credit Card') and the corresponding `Amount`.
* **Pie Chart:** Showing the proportional distribution of the **Top Categories** (e.g., 'subscription', 'Food', 'Transportation', etc.).
* **Scatter Plot:** Displaying the distribution of `Amount` across the **Top 10 Categories**.
* **Histogram:** Showing the **frequency distribution of `Amount`** for the first 10 rows of the dataset.
* **Box & Whisper Plot:** Analyzing the overall distribution and outliers of `Amount` within a specified range (e.g., $0 to $200).
* **Area Plot:** Visualizing the cumulative sum of `Amount` by **Top 40 Subcategories**.
* **Radar Plot:** Showing the mean `Amount` values for the **Top 10 Categories**.
* **Density Plot:** Illustrating the overall probability density function of the `Amount` column.

---

## Getting Started

### Prerequisites
The project uses standard Python data science libraries.
* Python 3.11
* Jupyter Notebook or Google Colaboratory

### Dependencies
You will need the following Python libraries:
* `pandas` (for data manipulation)
* `matplotlib.pyplot` (for plotting)
* `seaborn` (for advanced plotting)
* `sklearn` (for scaling and feature selection methods)
* `numpy` (for numerical operations, used in Decimal Scaling)

You can install them using pip:
```bash
pip install pandas matplotlib seaborn scikit-learn numpy
