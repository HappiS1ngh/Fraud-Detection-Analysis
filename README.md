Fraud Detection Analysis (Audit)
Project Overview
Fraudulent transactions can pose significant financial and reputational risks to organizations. This project demonstrates how data analytics techniques can be utilized to detect anomalies in financial transaction data, identify potential fraud, and provide insights for auditing purposes.

This analysis leverages Benford's Law to detect irregularities in the distribution of transaction amounts and employs statistical methods like Z-score-based outlier detection to flag transactions that deviate significantly from the norm. By combining these techniques, this project aims to provide a robust, data-driven approach to fraud detection in the field of auditing.

Objective
To detect fraudulent transactions in a dataset using:

Benford's Law: Analyze the distribution of the first digits in transaction amounts to flag potential anomalies.
Outlier Detection: Identify unusually high or low transaction amounts using statistical measures like Z-scores.
What This Project Does
Data Cleaning and Preparation

Loads a dataset of financial transactions.
Cleans and validates the data to ensure consistency and readiness for analysis.
Benford's Law Analysis

Applies Benford's Law to transaction amounts.
Compares the actual distribution of the first digits in transaction amounts to the expected distribution defined by Benford's Law.
Visualizes the results through a bar chart to highlight deviations.
Outlier Detection

Calculates the Z-score for each transaction amount.
Flags transactions as outliers if their Z-scores fall outside the standard threshold (greater than ±3).
Saves the flagged transactions to a separate CSV file for further investigation.
Visualization and Reporting

Generates a bar chart comparing actual vs. expected distributions for Benford's Law analysis.
Outputs a clean dataset of flagged transactions for auditors to review.
Tools Used
Python: Core programming language for data manipulation and analysis.
Pandas: Data manipulation and preprocessing.
Matplotlib: Visualization of Benford's Law analysis results.
NumPy: Statistical computations for outlier detection.
Deliverables
Dataset:

Fraud_Detection_Transactions_Corrected.csv
A dataset containing 500 transactions for analysis.
Visualization:

Benfords_Law_Analysis.png
A bar chart comparing the actual distribution of first digits in transaction amounts to the expected Benford's Law distribution.
Outlier Transactions:

Outlier_Transactions.csv
A file containing all transactions flagged as outliers based on Z-score analysis.
Python Script:

Fraud_Detection_Analysis.py
A Python script to automate fraud detection analysis using Benford's Law and statistical outlier detection.
How It Works
Step 1: Load the Dataset

The dataset includes transaction details such as Transaction ID, Amount, Customer ID, Vendor ID, and Payment Method.
Step 2: Perform Benford's Law Analysis

Analyze the distribution of the first digits in transaction amounts.
Flag significant deviations from the expected Benford's Law distribution.
Step 3: Detect Outliers

Use the Z-score method to identify unusually large or small transaction amounts.
Transactions with Z-scores greater than ±3 are flagged as potential outliers.
Step 4: Save Results

Save flagged transactions as a separate dataset for auditors to review.
Visualize results for Benford's Law analysis and save the chart for documentation.
Results
Benford's Law Analysis: Successfully visualized transaction patterns and flagged anomalies where the actual distribution deviated significantly from the expected pattern.
Outlier Detection: Identified and saved transactions with unusually high or low amounts to assist auditors in fraud investigation.
