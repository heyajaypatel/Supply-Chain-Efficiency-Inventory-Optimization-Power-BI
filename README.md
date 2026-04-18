# Supply Chain Efficiency & Inventory Optimization | Power BI

## 🎯 Project Objective
The objective of this project is to provide operations managers and procurement teams with a real-time command center for supply chain health. By analyzing inventory turnover, supplier lead times, and stockout frequency, this dashboard helps businesses maintain the delicate balance between meeting customer demand and minimizing excess inventory costs.

## 📊 Key Supply Chain Metrics (KPIs)
* **Total Inventory Value:** The total capital tied up in stock.
* **Inventory Turnover Ratio:** How many times a company has sold and replaced its inventory during a specific period.
* **On-Time Delivery %:** The reliability of suppliers in meeting delivery deadlines.
* **Stockout Count:** Frequency of instances where demand could not be met due to zero stock.
* **Reorder Point Status:** Visual alerts for items that have fallen below the safety stock threshold.

---

## 🛠️ Technical Workflow

### 1. Data Cleaning & Transformation (Power Query)
* **ETL Process:** Standardized SKU naming conventions, handled missing lead-time data, and merged supplier performance records with inventory logs.
* **Calculated Columns:** Built logic to determine "Days of Cover" (how long current stock will last based on average sales).

### 2. Data Modeling (Star Schema)
* **Structure:** Implemented a Star Schema connecting Inventory Fact tables with Dimension tables for Warehouses, Suppliers, and Product Categories.
* **Time Intelligence:** Integrated a `DateTable` to monitor seasonal fluctuations in inventory demand and supplier delays.

### 3. DAX Analysis & Optimization Logic
* **Stock Status Logic:** Created dynamic measures to label products as "Overstocked," "Healthy," or "Critical" based on current levels vs. reorder points.
* **Forecast Accuracy:** Developed measures to compare actual sales against predicted demand to refine future inventory orders.

---

## 💡 Business Insights
* **Working Capital Optimization:** Identified specific product categories where inventory is sitting idle for too long, freeing up cash flow.
* **Supplier Risk Assessment:** Pinpointed suppliers with high delay rates, allowing for more informed contract negotiations.
* **Stockout Prevention:** Established early-warning alerts for high-demand items, reducing the risk of lost sales.

## 📸 Dashboard Preview
> **Note to Recruiter:** This dashboard is optimized for operational efficiency, featuring high-visibility alerts and drill-down capabilities for warehouse-level details.

<img width="1920" height="1080" alt="Screenshot 2026-04-18 171145" src="https://github.com/user-attachments/assets/2b06982e-c053-4fcd-93d0-88c55c9b1ec3" />


## 🚀 How to Use
1. Clone this repository.
2. Open the `.pbix` file in **Power BI Desktop**.
3. Link the source files from the `Data/` folder.
4. Interact with **Slicers** (Warehouse Location, Supplier, Category) to analyze specific operational segments.

---
**Target Job Roles:** Supply Chain Analyst | Operations Manager | Inventory Planner | Procurement Analyst | Logistics Coordinator.
