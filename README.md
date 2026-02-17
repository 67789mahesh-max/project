# 🛒 Enterprise Data Analytics Pipeline (Medallion Architecture)

## 📌 Project Overview
This project demonstrates an **End-to-End Data Engineering & Analytics solution**. Unlike standard analysis projects, this repository implements a **Medallion Architecture** (Bronze/Silver/Gold layers) to simulate a real-world enterprise data environment.

The goal was to take raw, unstructured data, process it through a rigorous cleaning pipeline, and deliver a high-performance Power BI dashboard for business intelligence.

---

## 🏗️ Technical Architecture: The Medallion Model
I structured the data processing pipeline into three distinct layers to ensure data quality and scalability:

### 🥉 Bronze Layer (Raw Data)
* **Folder:** `bronze.layer/` *(Note: Raw ingestion)*
* **Function:** Acts as the landing zone for raw data ingestion.
* **State:** Data is kept in its original format (immutable) to ensure a single source of truth.

### 🥈 Silver Layer (Cleaned & Conformed)
* **Folder:** `silver.layer/`
* **Function:** Data is cleaned, filtered, and standardized.
* **Key Actions:**
    * Removed duplicates and handled null values.
    * Standardized data types and column naming conventions.
    * Enriched data for analytical relevance.

### 🥇 Gold Layer (Business Ready)
* **Folder:** `gold.layer/`
* **Function:** Aggregated data optimized for reporting and machine learning.
* **Output:** Star Schema models ready for Power BI ingestion.

---

## 🛠️ Tools & Technologies
* **Data Processing:** SQL / Python (Pandas)
* **Visualization:** Microsoft Power BI
* **Data Modeling:** Star Schema Design
* **Version Control:** Git & GitHub

## 🚀 Key Insights
* **Data Quality:** Successfully transformed unstructured raw inputs into a 100% clean analytical dataset.
* **Performance:** Optimized the data model in the Gold layer to reduce report loading time.
* **Business Value:** The dashboard highlights key sales trends, identifying top-performing categories and seasonal spikes.

## 📂 How to Run This Project
1.  Clone the repository.
2.  Navigate to the `datasets` folder to view the source files.
3.  Open `visualization.pbix` in **Power BI Desktop** to interact with the full dashboard.
