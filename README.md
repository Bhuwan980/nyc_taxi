# 🚕 NYC Taxi Data Pipeline (Batch Analytics)

This project demonstrates how to build a modular and efficient batch data pipeline for analytical insights using industry-standard tools. It focuses on ingesting and transforming millions of taxi trip records from NYC to power dashboards and reduce latency in querying.

---

## 🏗️ Project Architecture

The pipeline uses a hybrid **ELT + ETL** strategy:

- **ELT Phase**: Extracts data from the NYC trip data API, loads it into a staging PostgreSQL database, and transforms it using **dbt** for analytical modeling.
- **ETL Phase**: Pulls modeled data with **PySpark**, performs aggregation and further transformation, and loads the output into a serving database for visualization.
- **Storage**: Final datasets are stored on **Amazon S3** and queried using dashboards for business insights.

---

## 🔧 Tech Stack

- **Data Orchestration**: Apache Airflow  
- **Infrastructure**: Docker, Terraform  
- **Transformation & Modeling**: PySpark, dbt  
- **Storage**: PostgreSQL, Amazon S3  
- **Scripting**: Python, Boto3  
- **Visualization**: Looker Studio  

---

## 📦 How to Run Locally

1. **Clone the repository**  
```bash
git clone https://github.com/bhuwan980/nyc_taxi.git
cd NYC-Taxi-Trip-Data-Pipeline
