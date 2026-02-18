Enterprise Data Quality Governance & Validation Automation (Excel + Power Query + VBA)

🔎 Overview
This project is a corporate-grade Data Quality Control & Governance Automation System built in Excel using Power Query, relational modeling logic, and VBA-driven alert automation.
It simulates a real-world enterprise reporting environment where transaction data is divided year-wise (2023, 2024, 2025) and validated against structured dimension tables.

🏢 Real Corporate Problem Solved
In real organizations:
New transactions are added regularly
Master data (Customers, Products, Stores) may not be updated
Reports are generated without validation
Decision-makers rely on inaccurate data
This automation prevents that risk by validating referential integrity before reporting.

🧩 Data Architecture (Star Schema Logic)
✔ Dimension Tables (Unique IDs)
Customer Table (CustomerID + Details)
Product Table (ProductID + Details)
Store Table (StoreID + Details)
Each dimension table contains unique values only.
✔ Fact Table (Transactions)
Divided year-wise: 2023 / 2024 / 2025
Contains CustomerID, ProductID, StoreID
All dimensions are connected to transactions via their respective IDs

⚙️ Automation Logic
If:
A new transaction is added in 2025
And its Customer/Product/Store ID does NOT exist in respective dimension table
Then:
🚨 It is flagged as an error
 📌 Shown in dedicated sheets:
ERR_MISSING_CUSTOMER
ERR_MISSING_PRODUCT
ERR_MISSING_STORE

📊 A Data Quality Dashboard automatically updates on refresh:
Total Transactions
Total Errors
Valid Transactions
Error %
Data Health %
Health Status (Healthy / Warning / Critical)

📧 Smart Email Alert Automation
🔘 Email Button (VBA Macro)
Opens Outlook automatically
Pre-filled subject & message
Sends alert when Data Health ≤ 98%
Shows “Healthy” message when ≥ 98%
This simulates corporate data governance escalation workflows.

💡 Key Features
✔ Year-wise incremental transaction structure
 ✔ Referential integrity validation
 ✔ Automated error detection
 ✔ CEO-friendly Data Quality Dashboard
 ✔ Outlook Email Alert Integration
 ✔ One-click refresh
 ✔ Structured audit visibility

🛠 Tools & Skills Used
Microsoft Excel
Power Query
Relational Data Modeling
VBA Automation
Data Validation Logic
Conditional Formatting
Governance KPI Design
