# Customer Shopping Behavior Analysis

## Project Description

This project analyzes customer shopping behavior using transactional data containing 3,900 purchase records across multiple product categories. The objective is to explore customer demographics, spending patterns, subscription behavior, and product performance using Python, MySQL, and Power BI.

---

## Dataset Information

The dataset consists of 3,900 rows and 18 columns.

Key attributes include:

* Customer demographics: Age, Gender, Location, Subscription Status
* Purchase details: Item Purchased, Category, Purchase Amount, Season, Size, Color
* Shopping behavior: Discount Applied, Promo Code Used, Previous Purchases, Frequency of Purchases, Review Rating, Shipping Type

There were 37 missing values in the Review Rating column, which were handled during preprocessing.

---

## Tools and Technologies

* Python
* MySQL
* Power BI
* Jupyter Notebook

---

## Project Workflow

### 1. Data Preprocessing (Python)

* Loaded the dataset using Pandas
* Performed exploratory data analysis using df.info() and df.describe()
* Handled missing values in the Review Rating column using median imputation by product category
* Standardized column names to snake_case
* Created derived features:

  * age_group
  * purchase_frequency_days
* Removed redundant column (promo_code_used) after consistency check
* Exported cleaned data for SQL analysis

All preprocessing steps are documented in:

* `customer behavior.ipynb`

---

### 2. Business Analysis (MySQL)

Structured queries were written in MySQL to analyze:

* Revenue by gender
* High-spending discount users
* Top-rated products
* Shipping type comparison
* Subscribers vs non-subscribers
* Discount-dependent products
* Customer segmentation (New, Returning, Loyal)
* Top products per category
* Relationship between repeat purchases and subscriptions
* Revenue by age group

All SQL queries are available in:

* `customer bahvior analysis.sql`

---

### 3. Dashboard Development (Power BI)

An interactive Power BI dashboard was developed to visualize:

* Revenue distribution
* Customer segmentation
* Subscription impact
* Product performance
* Shipping preferences

Dashboard file:

* `customer behavior analysis.pbix`

---

## Project Files

The project directory contains:

* `customer_shopping_behavior.csv` – Raw dataset
* `customer behavior.ipynb` – Python preprocessing and EDA
* `customer bahvior analysis.sql` – MySQL queries
* `customer behavior analysis.pbix` – Power BI dashboard
* `Customer Behavior Analysis Report.pdf` – Final project report

---



* Improve the structure to look more professional for recruiters
