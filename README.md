# E-Commerce Sales Performance Dashboard

## 📊 Project Overview
This project is an end-to-end Data Analysis project focused on an e-commerce dataset for **E-Com Express**. The dashboard provides actionable insights into sales trends, product performance, and delivery efficiency to help stakeholders make data-driven decisions.

## 🖼️ Dashboard Preview
![Dashboard Preview](Screenshot/Screenshot1.png)
*Note: This project is currently in active development. Phase 1 (Core Metrics) is complete.*

---

## 🛠️ Tech Stack & Skills
* **Tool:** Power BI Desktop
* **Data Cleaning:** Power Query (ETL)
* **Data Modeling:** Star Schema (1-to-many relationships)
* **Calculations:** DAX (Data Analysis Expressions)

---

## 🚀 Key Features & Milestones

### 1. Data Transformation (ETL)
* Cleaned and standardized customer data (consistent capitalization, name merging).
* Handled inconsistent "Operating System" data using **Conditional Columns**.
* Managed null values in delivery dates specifically for cancelled orders to maintain data integrity.

### 2. Data Modeling
* Connected `Customers`, `Products`, and `Orders` tables via unique identifiers.
* Optimized model performance by using the `RELATED` function instead of merging large tables.

### 3. DAX & Analytics
Created custom measures to track business health, including:
* **Total Sales:** `$ \text{SumX}(\text{Orders}, \text{Quantity} \times \text{Related}(\text{Price})) $`
* **AOV (Average Order Value):** To measure consumer spending behavior.
* **Cancellation Rate:** A critical KPI tracking the 29.7% of lost orders to identify friction points.

---

## 📈 Current Project Status
- [x] **Phase 1: Foundation** - Data cleaning, modeling, and primary KPI cards.
- [x] **Phase 2: Sales Trends** - Time-series analysis and product distribution.
- [ ] **Phase 3: Customer Insights** - Deep dive into regional performance (In Progress).
- [ ] **Phase 4: Cancellation Analysis** - Root cause analysis for lost revenue (Planned).

---

## 📂 How to Use
1.  Clone this repository.
2.  Open the `E-Commerce_Analysis.pbix` file using **Power BI Desktop**.
3.  Ensure the data source paths in Power Query point to the `/Data` folder in this repo.
