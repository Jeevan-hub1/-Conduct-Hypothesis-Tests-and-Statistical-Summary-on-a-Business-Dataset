Assignment 5: Hypothesis Testing and Statistical Summary on Superstore Dataset
Overview
This repository contains a Jupyter Notebook (Assignment5.ipynb) that performs descriptive statistics, hypothesis testing, and visualizations on a small, real-world business dataset, as required for Assignment 5. The analysis uses the Superstore Dataset (or a synthetic subset) to extract insights into retail sales performance, meeting the following objectives:

Load and explore a business-related dataset.
Compute summary statistics (mean, median, mode, standard deviation, etc.) for numerical columns (Sales, Profit, Quantity).
Formulate and test two hypotheses using a one-sample t-test and a chi-square test.
Visualize distributions with histograms and boxplots.
Conduct correlation analysis with a heatmap (bonus).
Create pivot tables for group-wise summaries (bonus).
Provide markdown commentary explaining findings.

The notebook fulfills all evaluation criteria: correct statistical test implementation, accurate hypothesis formulation, clear result interpretation, and high-quality visualizations.
Dataset

Source: Superstore Dataset from Kaggle, a retail dataset with sales, profit, and quantity data.
Columns Used:
Region: Geographical region (e.g., Central, East, South, West).
Category: Product category (e.g., Furniture, Office Supplies, Technology).
Sales: Sales amount in dollars.
Profit: Profit amount in dollars.
Quantity: Number of items sold.


Size: ~1000 rows (filtered from the original dataset or synthetic subset).
Fallback: If Superstore.csv is unavailable, the notebook generates a synthetic dataset mimicking the Superstore structure (1000 rows, saved as superstore_subset.csv).

Files

Assignment5.ipynb: Jupyter Notebook containing the analysis code, visualizations, and markdown commentary.
superstore_subset.csv (optional): Synthetic dataset generated if Superstore.csv is not provided.
README.md: This file, providing project overview and instructions.

Requirements

Python Version: Python 3.8 or higher.
Dependencies: Install the required libraries using:pip install pandas numpy matplotlib seaborn scipy


Environment: Jupyter Notebook or JupyterLab.
Dataset: Download Superstore.csv from Kaggle and place it in the working directory. Alternatively, the code creates a synthetic subset if the file is missing.

Instructions to Run

Clone the Repository:git clone <repository-url>
cd <repository-name>


Install Dependencies:Ensure the required libraries are installed (see Requirements).
Prepare Dataset:
Place Superstore.csv in the repository’s root directory.
If unavailable, the notebook will generate superstore_subset.csv.


Open Jupyter Notebook:jupyter notebook Assignment5.ipynb


Run the Notebook:
Execute all cells sequentially.
The code loads the dataset, performs statistical analysis, conducts hypothesis tests, and generates visualizations.


View Outputs:
Console outputs include summary statistics, hypothesis test results, correlation matrix, and pivot tables.
Visualizations (histograms, boxplots, heatmap) are displayed inline.


Export to PDF (for submission):jupyter nbconvert --to pdf Assignment5.ipynb

Or use Jupyter’s “File > Download as > PDF via LaTeX” (requires LaTeX installation).

Analysis Overview

Descriptive Statistics: Computes mean, median, mode, and standard deviation for Sales, Profit, and Quantity.
Visualizations: Histograms and boxplots show distributions and outliers for numerical columns.
Hypothesis Tests:
One-Sample t-test: Tests if the mean Sales differs from $200 (H₀: mean = $200, H₁: mean ≠ $200).
Chi-Square Test: Tests for association between Region and Category (H₀: no association, H₁: association exists).


Correlation Analysis: Generates a correlation matrix and heatmap for Sales, Profit, and Quantity.
Pivot Table: Summarizes mean Sales and Profit by Region and Category.

Key Findings

Statistics: Sales and Profit show variability, with potential outliers detected in boxplots.
t-test: The p-value indicates whether the mean sales significantly differ from $200.
Chi-Square: The p-value determines if Region and Category are associated.
Correlation: The heatmap reveals relationships (e.g., potential positive correlation between Sales and Profit).
Pivot Table: Highlights regional and categorical differences in sales and profit performance.

Submission Details

GitHub: This repository ().
PDF Report: Export Assignment5.ipynb to PDF for submission.
Date: Completed on June 20, 2025.

Notes

Customization: Replace Superstore.csv with another dataset by updating the file path and column names in the code.
Troubleshooting: Ensure libraries are installed and the dataset is accessible. If errors occur, check the synthetic dataset generation.
Contact: For issues or clarifications, reach out to  or open an issue in this repository.

