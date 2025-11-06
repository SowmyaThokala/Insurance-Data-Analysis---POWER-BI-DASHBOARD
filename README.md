Dashboard Link: https://app.powerbi.com/groups/me/reports/ce2eaf25-6da5-4c27-a3c0-ea8c2caed621/519b2ed978d90040e49d?experience=power-bi

## Overview

This project presents a Power BI dashboard developed for **PRISM INSURANCE PVT. LTD.**, aimed at analyzing key insurance data such as policy details, claim amounts, coverage, and customer demographics. The report helps business stakeholders monitor performance, identify trends, and make informed decisions.


## Business Objective

The primary objective of this dashboard is to provide an analytical view of the company’s insurance operations. The report enables users to:

Track total premium, coverage, and claim amounts.
Analyze claim status across different categories.
Understand customer segmentation by gender and age group.
Monitor policy activity (active vs inactive).
Provide detailed data drill-through for deeper insights.
Enforce data security using role-based access (Row Level Security).


## Data Source and Setup

1. Created a SQL Server database named **`InsuranceDB`**.
2. Imported the dataset **`insurancedata`** into the database.
3. Connected Power BI Desktop to **InsuranceDB** using the SQL Server connector.
4. Loaded the data model into Power BI for transformation and visualization.


## Data Transformation and Modeling

Added a calculated column **“Age Group”** using conditional logic to categorize customers based on age.
Created a new column **“Active/Inactive”** using conditional logic to determine policy status based on the current date.
Ensured data model relationships were defined for accurate aggregation and analysis.


## Report Development in Power BI

## Slicers
Policy Number  
Claim Number  
Customer ID  

## Visuals and Components
**Title:** Added a text box with the heading *“PRISM INSURANCE PVT. LTD.”* under the *Insert* tab.
**Card Visuals:** Displayed Total Premium Amount, Total Coverage Amount, and Total Claim Amount.
**Multi-row Card:** Represented the number of Male and Female customers.
**Ribbon Chart:** Illustrated Claim Status categories and their respective counts.
**Stacked Bar Chart:** Showed Premium Amount by Policy Type.
**Line Chart:** Displayed Claim Amount across different Age Groups.
**Donut Chart:** Represented Active vs Inactive Policies.
**Matrix Visual:** Showed Policy Type, Claim Status, and Coverage Amount.

## Page 2 – Detailed Data View

Added a Table visual containing all columns from the dataset for comprehensive record viewing.
Enabled **Drill Through** functionality based on **Policy Type** for detailed insights.

## Row Level Security (RLS)

To maintain data confidentiality, **Row Level Security** (RLS) was implemented with the following roles:

**Health Role:** Access limited to Health Policy Type.
**Travel Role:** Access limited to Travel Policy Type.

This ensures that users can only view data relevant to their assigned policy category.

## Deployment and Refresh

Published the Power BI report to the **Power BI Service**.
Configured a **scheduled refresh** for the semantic model to ensure the dashboard remains up to date with the latest data.

## Key Insights

Overview of financial metrics such as Total Premium, Coverage, and Claim Amounts.
Gender-based customer distribution.
Policy activity monitoring (Active vs Inactive).
Claim trend analysis by status and age group.
Policy performance tracking by type.

## Tools and Technologies Used

 ## Tool / Technology / Purpose 

| **Microsoft SQL Server** | Database creation and data storage |
| **Power BI Desktop** | Data modeling, visualization, and report building |
| **Power BI Service** | Report publishing, scheduling refresh, and Row Level Security implementation
