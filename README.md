# Customer Behavior Dashboard


📍 Project Overview

This project analyzes customer shopping behavior using transactional data from 3,900 purchases across multiple product categories. The goal is to uncover insights about spending patterns, customer segments, product preferences, and subscription behavior to support data-driven business decisions.

📊 Dataset Summary

Rows: 3,900

Columns: 18

Key Features:

Demographics: Age, Gender, Location, Subscription Status

Purchase details: Item Purchased, Category, Purchase Amount, Season, Size, Color

Behavior: Discount Applied, Previous Purchases, Promo Code Used, Rating, Frequency, Shipping Type

Missing Data: 37 values in Review Rating (handled during cleaning)

🧹 Exploratory Data Analysis (Python)

Performed using Pandas, NumPy, Seaborn, and Matplotlib:

Loaded and explored dataset (info(), describe())

Handled missing values (imputed Review Rating using category-wise median)

Renamed columns to snake_case for clarity

Feature engineering:

age_group (binned ages)

purchase_frequency_days

Data consistency checks (dropped redundant promo_code_used)

Connected Python to PostgreSQL

Loaded cleaned data into database for SQL analysis

🗃 SQL Analysis (PostgreSQL)

Key business questions answered:

Revenue by gender

High-spending discount users

Top 5 products by average review rating

Standard vs Express shipping revenue comparison

Subscribers vs non-subscribers (average spend + total revenue)

Products most dependent on discounts

Customer segmentation: New, Returning, Loyal

Top 3 products per category

Repeat buyers & their subscription likelihood

Revenue contribution by age group

📊 Power BI Dashboard

An interactive dashboard was created in Power BI to visualize: 
## 🎥 Dashboard Interaction Demo
https://github.com/YogaSelvakumar/Customer-Shopping-Behavior-Analysis/blob/main/Video%20Project%201.mp4


KPIs: Total customers, Avg Purchase Amount, Avg Review Rating

Revenue by Category

Sales by Age Group

Subscription Status Split

Shipping Type Preferences

Category & Demographic filters

📌 Business Recommendations

Promote subscription benefits to boost conversion

Introduce loyalty rewards for repeat customers

Review discount strategy to protect profit margins

Highlight top-rated and best-selling products

Target marketing toward high-revenue age groups

🚀 How to Run This Project

Clone this repository

Install dependencies using requirements.txt

Run the Python notebook for data cleaning & EDA

Import cleaned data into PostgreSQL using SQL scripts

Open the Power BI file (.pbix) to explore the dashboard

Refer to the PPT included for a complete walkthrough
