# E-Commerce Sales Intelligence Platform

## 📌 Project Overview
This project is an interactive, high-fidelity business intelligence dashboard developed in Power BI Desktop. The platform ingests relational retail datasets to deliver on-demand profit tracking, customer behavior analysis, and spatial-temporal operational insights to executive stakeholders.

## 📸 Dashboard Preview
<img width="1360" height="765" alt="Dashboard_screenshot" src="https://github.com/user-attachments/assets/d7f84117-197f-4e3d-865e-0d0a542203c4" />

*Snapshot reflecting Q4 performance metrics isolated for the state of Maharashtra.*

---

## 🏗️ Data Architecture & ETL Pipeline
The backend architecture of this project focuses on strict relational data modeling. Raw e-commerce data was ingested via two distinct files and normalized into a unified model:

### 1. Data Sources & Schema
*   **`Orders.xlsx` (Dimension Table):** Contains 500 unique records tracking overarching order metadata, including `Order ID`, `Order Date`, `CustomerName`, `State`, and `City`.
*   **`Details.xlsx` (Fact Table):** Contains 1,500 transactional records detailing the granular line-item metrics, including `Amount`, `Profit`, `Quantity`, `Category`, `Sub-Category`, `PaymentMode`, and `AOV` (Average Order Value).
*   **Data Modeling:** Engineered a 1-to-Many relational model linking the tables via the `Order ID` primary/foreign key to optimize query performance and enable cross-filtering.

### 2. Semantic Layer & Analytics
Developed a robust semantic layer to calculate dynamic metrics across various dimensions:
*   **Temporal Intelligence:** Sliced performance by financial quarters (Q1–Q4) and granular monthly trends (e.g., tracking the profit dip in December against November highs).
*   **Categorical Profitability:** Isolated top-performing product categories, identifying *Electronic Games* and *Printers* as primary profit drivers.
*   **Consumer Behavior:** Mapped purchase volume against specific payment methods and ranked top individual customers (e.g., Gopal, Uudhav) by lifetime value.

## 📊 Core Dashboard Features
*   **Executive KPI Banner:** High-level dynamic tracking of Total Amount, Total Profit, Total Quantity, and Average Order Value (AOV).
*   **Visual Drill-Down Layouts:** Hierarchical matrices and charts allowing stakeholders to drill from regional state performance (e.g., Maharashtra) down to individual product category margins.
*   **Interactive Slicers:** Cross-filtering enabled across all visual layers for on-demand spatial (State) and temporal (Quarter) analysis.

## 📂 Repository Contents
*   `Ecommerce sale Dashboard.pbix` - The complete Power BI project file containing the data model, DAX measures, and frontend UI.
*   `Orders.xlsx` - Customer and localization dimension dataset.
*   `Details.xlsx` - Granular transactional fact dataset.
*   `Dashboard_screenshot.png` - High-resolution UI preview.

## 🛠️ Tech Stack
*   **Tool:** Power BI Desktop
*   **Backend:** Data Modeling (Relational 1:* Schema)
*   **Analytical Engine:** DAX (Data Analysis Expressions)
