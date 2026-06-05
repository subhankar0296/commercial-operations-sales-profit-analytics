# Commercial Operations & Profit Margin Optimization Engine

## 📋 Project Overview
This project focuses on translating raw transactional, product, and regional data into strategic business insights for an omni-channel retail operation. By engineering a relational schema across sales performance (`Fact`), product lines (`Product`), and distribution geography (`Location`), this engine isolates revenue leakage, evaluates marketing ROI, and tracks inventory turnover. 

The primary objective is to equip operations leadership and stakeholders with programmable database modules to dynamically analyze **Cost of Goods Sold (COGS)**, **Budget Margins**, and **Net Profitability** across different states[cite: 2].

---

## 🛠️ Tech Stack & Key Concepts
*   **Database Engine:** Microsoft SQL Server
*   **Advanced SQL Techniques:** Window Functions (`DENSE_RANK`), Hierarchical Aggregations (`ROLLUP`), Explicit Transaction Isolation (`ACID` compliance)[cite: 2]
*   **Database Programmability:** Stored Procedures, Scalar User-Defined Functions (UDFs), Table-Valued Functions (TVFs)[cite: 2]
*   **Business Intelligence Core:** Inventory Control, Profitability Modeling, Margin Risk Calculations[cite: 2]

---

## 📐 Database Schema Architecture
The project utilizes an optimized relational model consisting of three primary tables[cite: 2]:
1.  **`Location`:** Relational lookup containing geographic footprints (`Area_Code`, `State`)[cite: 2].
2.  **`Product`:** Product registry tracking classification metrics (`ProductID`, `Product`, `Product_Type`, `Type`)[cite: 2].
3.  **`Fact`:** Centralized transactional ledger recording operational metrics (`Sales`, `COGS`, `Profit`, `Inventory`, `Marketing`, `Total_Expenses`, `Date`) linked to dimensions[cite: 2].

---

## 🚀 Key Highlights & Advanced Implementation

### 1. Database Automation & Custom Programmability
To eliminate repetitive manual lookups, the database is embedded with custom programmable abstractions[cite: 2]:
*   **Scalar Functions:** Built an expansion module (`Increased_sale`) to dynamically forecast potential margins against a hypothetical 5% across-the-board sales increase[cite: 2].
*   **Table-Valued Functions:** Deployed an inline TVF (`Product_Type`) allowing dynamic, parameterized querying of product catalogs based on stakeholder preference[cite: 2].
*   **Stored Procedures:** Programmed a reusable stored procedure execution framework (`ProductType`) to isolate inventory categories efficiently[cite: 2].

### 2. Analytical Depth & Advanced Query Optimization
*   **Multi-Level Hierarchical Aggregations:** Leveraged the `ROLLUP` operator to generate complex multi-dimensional aggregates, rolling up transactional data from localized `ProductID` levels to weekly and grand-total layers simultaneously[cite: 2].
*   **Window Functions for Ranking:** Used `DENSE_RANK() OVER` partitioned logic to run dense sales-wise ranking profiles without gaps, removing statistical skew during performance benchmarking[cite: 2].
*   **Conditional Risk Frameworks:** Embedded logical evaluation trees (`CASE WHEN`) to instantly categorize product performance into a customized binary classification structure (`Profit` vs. `Loss` thresholds based on expense overheads)[cite: 2].

### 3. Data Integrity & Transaction Controls
*   Showcases standard enterprise risk management by enclosing structural updates within `BEGIN TRAN` block structures[cite: 2]. This guarantees data consistency by using safe `ROLLBACK` safety nets to preserve state history during volatile database modifications[cite: 2].

---

## 📊 Strategic Business Questions Answered
The analytical script provides explicit answers to critical operational metrics, including[cite: 2]:
*   Total marketing spend efficiency isolated by individual high-priority product keys[cite: 2].
*   State-by-state profit metrics mapping revenue peaks (e.g., isolating performance in Colorado)[cite: 2].
*   Average inventory levels grouped by product ID to prevent warehouse bloat and stockout anomalies[cite: 2].
*   Product margin health reporting tailored to flag product segments dropping below a target 100-unit index[cite: 2].

---

## 💻 How to Run the Scripts
1. Open **SQL Server Management Studio (SSMS)** or your preferred T-SQL terminal.
2. Execute the schema generation and dataset population scripts.
3. Run the analytical query batches sequentially to evaluate database performance, build the programmatic functions, and observe output metrics[cite: 2].
