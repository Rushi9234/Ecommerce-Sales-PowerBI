# E-Commerce Sales Intelligence Platform

## 📌 Project Overview
An interactive, high-fidelity business intelligence dashboard developed in Power BI Desktop. This platform ingests raw, high-volume transactional retail records and transforms them into an optimized Snowflake schema to deliver on-demand profit tracking and operational insights to executive stakeholders.

## 🏗️ Data Architecture & ETL Pipeline
Raw e-commerce data (sales, inventory, and localization variables) inherently contains structural anomalies. The backend architecture of this project focuses on strict data modeling:
1. **Extraction & Transformation (Power Query):** Cleaned raw datasets, resolved data type inconsistencies, and executed merge/append operations to unify siloed tables.
2. **Data Modeling:** Engineered a robust **Snowflake Schema**, normalizing dimension tables (Products, Regions, Customers) around a central transactional Fact table to optimize query performance and filter propagation.
3. **Semantic Layer (DAX):** Developed robust Data Analysis Expressions (DAX) to calculate advanced time-intelligence metrics, profit margins, and rolling averages.

## 📊 Dashboard Features
* **Executive KPI Tracking:** Top-level metrics for Total Revenue, Profit Margins, and Order Volume.
* **Visual Drill-Down Layouts:** Hierarchical matrices and charts allowing stakeholders to drill from regional performance down to individual product category margins.
* **Interactive Filtering:** Cross-filtering enabled across all visual layers for on-demand spatial and temporal analysis.

## 📂 Repository Contents
* `Ecommerce sale Dashboard.pbix` - The complete Power BI project file (contains the Power Query M code, DAX models, and frontend layouts).

## 🛠️ Tech Stack
* **Tool:** Power BI Desktop
* **Backend:** Power Query (M Language), Data Modeling (Snowflake Schema)
* **Analytical Engine:** DAX (Data Analysis Expressions)

## 💡 How to View
1. Ensure you have [Power BI Desktop](https://powerbi.microsoft.com/desktop/) installed on your machine.
2. Download the `Ecommerce sale Dashboard.pbix` file from this repository.
3. Open the file to explore the interactive visual canvas, the underlying data model view, and the DAX measures.
