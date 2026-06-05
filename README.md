# pyspark-dbt-project


# End-to-End Data Engineering Pipeline using Databricks, PySpark & dbt Cloud

## Project Overview

This project demonstrates an end-to-end Data Engineering pipeline built using Databricks, PySpark, Delta Lake, and dbt Cloud following the Medallion Architecture (Bronze, Silver, Gold).

The pipeline ingests raw customer data, performs data cleaning and transformation using PySpark, and builds analytics-ready datasets using dbt models.

---

## Architecture

Raw Data
→ Bronze Layer (Data Ingestion)
→ Silver Layer (Data Cleaning & Transformation)
→ Gold Layer (Business-Ready Data Models)
→ Analytics & Reporting

---

## Technologies Used

* Databricks
* PySpark
* Delta Lake
* Unity Catalog
* dbt Cloud
* SQL
* GitHub

---

## Medallion Architecture

### Bronze Layer

The Bronze layer stores raw ingested data from source files without major transformations.

Key Tasks:

* Read source CSV files
* Infer schema
* Load raw data into Delta tables
* Preserve source data integrity

### Silver Layer

The Silver layer performs data cleansing and transformation.

Key Tasks:

* Handle missing values
* Remove duplicates
* Standardize data types
* Apply business rules
* Improve data quality

### Gold Layer

The Gold layer contains business-ready datasets optimized for analytics and reporting.

Key Tasks:

* Aggregate metrics
* Create dimensional models
* Generate reporting tables
* Support BI and dashboard use cases

---

## dbt Implementation

dbt Cloud is used to:

* Build transformation models
* Manage SQL-based transformations
* Document data lineage
* Implement data quality tests
* Create reusable analytics models

Project Structure:

models/
tests/
snapshots/
macros/
dbt_project.yml

---

## Databricks Catalog Structure

pysparkdbt

├── bronze
├── silver
└── gold

This structure follows industry-standard Medallion Architecture principles.

---

## Repository Structure

```text
pyspark-dbt-project/

├── notebooks/
│   ├── bronze_ingestion
│   ├── silver_transformation
│
├── dbt/
│   ├── models/
│   ├── tests/
│   ├── snapshots/
│   ├── macros/
│   └── dbt_project.yml
│
├── screenshots/
│
└── README.md
```

---

## Key Learnings

Through this project I gained practical experience in:

* Data Engineering Fundamentals
* ETL / ELT Pipeline Development
* PySpark Data Processing
* Delta Lake Architecture
* Unity Catalog Management
* Data Modeling with dbt
* Git & GitHub Version Control
* Medallion Architecture Design

---

## Future Improvements

* Automated orchestration using Apache Airflow
* CI/CD integration with GitHub Actions
* Data quality monitoring
* Real-time streaming ingestion
* Dashboard integration using Power BI or Tableau

---

## Author

Emmanuel Nischay Gapti

Aspiring Data Engineer focused on Databricks, PySpark, dbt, Delta Lake, and modern Data Engineering practices.
