# Project Management Analytics – Data Cleaning & Performance Insights (Pandas)

## Overview

This project focuses on analyzing a project management dataset using Python (Pandas). The goal is to clean raw operational data, validate relationships between tables, and extract insights about project performance, client behavior, and team efficiency.

The dataset simulates real-world project operations including project managers, clients, budgets, delivery metrics, and performance indicators.

## Objectives

* Clean and standardize messy operational data
* Ensure data integrity across related tables
* Engineer meaningful business metrics
* Analyze performance across departments, regions, and priorities
* Identify trends in client behavior and project outcomes

## Data Cleaning Process

The dataset was prepared through several cleaning steps:

* Handling missing values:
    Addressed missing velocity and client_satisfaction values, especially for non-completed projects. These were either flagged, filled with rules, or excluded depending on analysis needs.
* Fixing data types:
    Converted date fields from strings into proper datetime formats for accurate time-based analysis.
* Outlier detection:
    Identified cases where actual_spend_usd exceeded budget by significant margins (e.g., >15%), and flagged them for review.
* Orphan record detection:
    Checked for employees not linked to any project using relational validation techniques.
* Foreign key validation:
    Verified that all project_manager_id values exist in the employees dataset to ensure referential integrity.
* Feature engineering:
    Created new columns such as:
    * Project overrun amount
    * Project duration (days)
    * Budget overrun percentage

## Analysis Performed

The cleaned dataset was used for multiple analytical tasks:

* Grouped data by department, region, and priority to compare performance patterns
* Ranked project managers by average client satisfaction
* Calculated budget burn rate per project type
* Identified clients with the highest project cancellation rates
* Built a correlation analysis between salary, team size, delivery velocity, and satisfaction

## Key Insights (to be updated after visualization)

* Patterns in project delivery efficiency across departments
* Relationship between team size and performance outcomes
* Client behavior trends related to cancellations
* Financial inefficiencies in specific project categories

## Tools Used

* Python
* Pandas
* NumPy (if used)
* Matplotlib / Seaborn (to be added in next phase)

## Next Steps

* Add visual dashboards and charts
* Build interactive insights summary
* Improve feature engineering for predictive modeling
* Extend dataset for time-series forecasting

## Project Value

This project demonstrates practical skills in:

* Data cleaning and validation
* Business-focused analytics
* Working with relational datasets
* Extracting actionable insights from raw operational data
