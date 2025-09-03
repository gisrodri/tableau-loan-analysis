# Financial Risk Analysis Dashboard - Lending Club

This repository contains the data preparation phase for an interactive financial risk analysis dashboard built with Tableau. The project involves cleaning and transforming a large dataset from Lending Club to create a focused and efficient data source for visualization.

---

## 🚀 Interactive Dashboard

The final, interactive dashboard is published on Tableau Public. You can view and interact with it here:

**[View Dashboard on Tableau Public](https://public.tableau.com/app/profile/giseli.rodrigues/viz/FinancialRiskAnalysis-LendingClub/Dashboard1 )**

*(Note: Replace the URL above with the actual link to your dashboard once it's published. You can find this link by going to your dashboard on Tableau Public and clicking the "Share" button.)*

---

## 📋 Project Overview

The goal of this project is to analyze loan data to identify key drivers of loan defaults. The dashboard provides insights into:
*   Overall portfolio performance and default rates.
*   Risk profiles based on loan grades and purposes.
*   Geographical distribution of risk across a map.

---

## 🛠️ Data Preparation

The data preparation is done in the Jupyter Notebook located in the `notebooks/` folder. The process includes:

1.  **Optimized Loading:** Reading a multi-gigabyte CSV file efficiently by selecting only relevant columns.
2.  **Data Cleaning:** Handling missing values, correcting data types, and standardizing text fields (e.g., `emp_length`).
3.  **Feature Engineering:** Creating a key `loan_condition` column ('Good' vs. 'Bad') to simplify risk analysis.
4.  **Final Output:** Exporting a clean, analysis-ready CSV file to be used as the data source in Tableau.

### Data Source
The data used is the **[Lending Club Loan Data](https://www.kaggle.com/datasets/wordsforthewise/lending-club )** from Kaggle.

---

## ⚙️ How to Replicate

This project uses the Kaggle API to download the necessary data.

1.  **Set up your environment:**
    *   Clone this repository.
    *   Create a virtual environment and install the required packages (e.g., `pip install pandas numpy kaggle`).
    *   Ensure your Kaggle API credentials (`kaggle.json`) are set up correctly on your machine.

2.  **Run the data preparation notebook:**
    *   Open and run the `notebooks/01-lendingclub-data-prep.ipynb` notebook.
    *   The notebook will automatically download the required compressed data file (`accepted_2007_to_2018Q4.csv.gz`) from Kaggle using the API.

3.  **Find the output:**
    *   After the notebook runs successfully, it will generate the final, clean dataset at `data/cleaned_loan_data.csv`..
