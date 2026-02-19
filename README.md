# Supermarket-Data-Analysis
# Project Overview 
This project analyzes three years of supermarket transaction data to answer specific business-driven questions using Python and MongoDB.

The objective was to perform structured data cleaning, targeted aggregation, and reproducible analysis while maintaining data integrity and traceability.

The final deliverables include:

A cleaned transaction dataset

A summary report of findings

A MongoDB-ready dataset for further database integration

# Repository Structure
Supermarket_Data_Analysis.ipynb
cleaned_supermarket_transactions.csv
Supermarket_Analysis_Summary.txt
README.md

# Technologies Used
Python 3
Pandas
Pymongo
MongoDB
Google Colab

# Business Questions Adrressed
The analysis answers the following:

What is the total quantity of apples purchased using cash?

What is the total cash amount spent on apples?

What is the total amount spent by non-member customers at the Bakershire store?

# Data Preparation and Cleaning
Data Preparation & Cleaning

The following preprocessing steps were applied:

Removed unnecessary columns (e.g., Unnamed: 0)

Standardized text fields (case normalization and whitespace trimming).

Verified unique product naming conventions.

Ensured deterministic filtering logic.

Checked for null values.

Validated dataset structure before aggregation.

Re-exported cleaned dataset for reproducibility.

A critical correction was made during validation:

The dataset used "apple" (singular), not "apples" — this adjustment ensured accurate aggregation.

# METHODOLOGY
Filtering logic was implemented using explicit conditional selection in Pandas:

Product-based filtering

Payment method filtering

Customer-type filtering

Store-based filtering

Aggregation using .sum()

All results are reproducible and derived directly from transactional records without inferred assumptions.

# MongoDB Intergration
The cleaned dataset was:

Reloaded into the notebook.

Modified to use a proper _id field.

Prepared for insertion into MongoDB.

Validated for null consistency before database loading.

This enables further query expansion and scalable database analytics.

# FUTURE IMPROVEMENTS
Add exploratory data analysis (EDA) visualizations.

Implement automated validation tests.

Introduce aggregation pipelines directly within MongoDB.

Add KPI dashboards.

Parameterize analysis for dynamic querying.


