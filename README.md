# Retail Sales Data Cleaning & Quality Analysis

## 📌 Project Overview

This project focuses on understanding, assessing, cleaning, and validating a retail sales dataset before using it for further analysis.

The analysis was performed using **Python and Pandas**, with a focus on identifying data quality issues and preparing the dataset for reliable sales analysis.

## 📊 Dataset

The project uses an **Online Retail** sales dataset containing transaction-level information.

The dataset includes information such as:

* Invoice Number
* Product Description
* Quantity
* Invoice Date
* Unit Price
* Customer ID
* Country

## 🔍 Data Quality Checks

The dataset was examined for:

* Missing values
* Duplicate records
* Negative and zero quantities
* Non-positive prices
* Incorrect data types

## 🧹 Data Cleaning

The following cleaning steps were performed:

* Converted `InvoiceDate` to datetime format.
* Removed duplicate records.
* Excluded transactions with quantities less than or equal to zero from the sales analysis.
* Excluded records with unit prices less than or equal to zero.
* Retained missing `CustomerID` values because the transactions still contain useful sales information.

## ⚙️ Feature Engineering

Two useful features were created:

* **Revenue** = Quantity × UnitPrice
* **InvoiceMonth** – used to support monthly sales trend analysis.

An `OrderType` feature was also created to identify sales and cancellation transactions based on the invoice number.

## ✅ Data Validation

After cleaning, the dataset was validated again to confirm that:

* Duplicate records were removed.
* Invalid quantities were excluded.
* Invalid prices were excluded.
* Data types were correctly formatted.
* Missing values were reviewed.

## 🛠️ Technologies Used

* Python
* Pandas
* NumPy
* Google Colab
* Jupyter Notebook

## 📁 Project Files

* `retail_task_.ipynb` — Data cleaning and quality analysis notebook.
* `online_retail_cleaned.csv` — Cleaned dataset generated from the analysis.

## 🎯 Outcome

After the cleaning and validation process, the dataset was prepared for further retail sales analysis and business insights.
