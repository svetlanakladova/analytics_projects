## Taxi Data Pipeline

**Project Overview**

In this project, I built an automated data pipeline for processing Yandex Taxi trip data using PySpark, Airflow, and ClickHouse.

The goal was to automate daily data aggregation and create a table with key business metrics for different payment types. The pipeline checks whether a new data file appears in S3 storage, runs a Spark job for processing the data, and then loads the final aggregated table into ClickHouse.

During the project, I worked with distributed data processing in Spark, created an Airflow DAG for orchestration, configured connections to cloud storage and ClickHouse, and automated the entire workflow from data ingestion to analytical output.

The final table can be used by analytics or finance teams for reporting and dashboarding.


**Key areas of analysis:**

- Developed ETL workflows using Airflow and PySpark
- Automated data processing and reporting pipelines

---

**Tools & Technologies**

`PySpark` `Apache Airflow` `ClickHouse` `ETL Pipelines`
