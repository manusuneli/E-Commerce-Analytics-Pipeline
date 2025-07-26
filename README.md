# Real-Time E-Commerce Analytics Pipeline using PySpark & GCP

This project showcases an **end-to-end big data pipeline** for real-time analytics on e-commerce data using **PySpark**, **Google Cloud Platform (GCP)**, and various cloud-native services.

## 📌 Project Objective

To simulate a real-world e-commerce data processing scenario by building a scalable data pipeline that:
- Ingests raw transactional data
- Performs cleaning, transformation, and enrichment
- Serves analytical data layers for reporting
- Visualizes business insights using BI tools

---

## 🧰 Tech Stack

| Layer         | Tools & Services                             |
|---------------|----------------------------------------------|
| Programming   | Python, PySpark                              |
| Cloud         | Google Cloud Platform (GCP)                  |
| Processing    | Google Cloud Dataproc (Apache Spark)         |
| Storage       | Google Cloud Storage (GCS)                   |
| Orchestration | Apache Airflow (Cloud Composer)             |
| Visualization | Google Data Studio, Power BI (optional)      |
| Data Formats  | CSV, Parquet                                 |

---

##  Architecture

[ Raw Data ] --> [ GCS Bucket ]
↓
[ Dataproc Cluster (PySpark) ]
↓
[ Cleaned & Enriched Data in GCS ]
↓
[ Analytical Views Layer ]
↓
[ Visualization in Data Studio ]


---

## ⚙️ Pipeline Steps

1. **Data Ingestion**
   - Raw e-commerce transaction data ingested into Google Cloud Storage.

2. **Data Processing**
   - PySpark jobs on Dataproc to:
     - Clean nulls, remove duplicates
     - Handle schema inconsistencies
     - Join with product & customer metadata

3. **Data Transformation**
   - Use Spark SQL and DataFrames for:
     - Aggregation, enrichment
     - Window functions, partitioning
     - Optimized joins (broadcast, bucketing)

4. **Data Serving**
   - Final transformed datasets written to a curated layer in GCS (or BigQuery).

5. **Visualization**
   - Dashboards built in Google Data Studio to analyze key metrics like:
     - Top-selling products
     - Revenue by region
     - Conversion trends over time

---

##    Sample Outputs

- ✅ Enriched product-sales tables
- ✅ Partitioned Parquet files for analytics
- ✅ BI-ready dashboards with KPI metrics

---

## 🚀 Key Learnings

- How to scale distributed data processing using PySpark on GCP
- Real-time data handling with managed cloud services
- Best practices for pipeline performance and optimization
- CI/CD for PySpark jobs using Airflow orchestration

---



