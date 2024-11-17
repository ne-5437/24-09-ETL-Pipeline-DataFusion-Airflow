# ETL Pipeline with Apache Airflow and Google Cloud Data Fusion

This repository contains an ETL pipeline implementation that integrates **Apache Airflow** for orchestration and **Google Cloud Data Fusion** for data processing. The pipeline extracts employee data from a CSV file, processes it using Google Cloud Data Fusion, and loads it into a target destination, such as BigQuery or Cloud Storage.

## Project Structure

etl-pipeline/
├── dags/
│   └── employee_data_etl.py     # The Airflow DAG script
├── scripts/
│   └── extract.py               # Python script to extract data from CSV
├── data/
│   └── employee_data.csv        # Sample data CSV
└── README.md                    # Project documentation

## Prerequisites

1. **Apache Airflow**: For orchestrating the ETL pipeline.
2. **Google Cloud Platform (GCP)**: Required for running Google Cloud Data Fusion and storing data in Cloud Storage or BigQuery.
3. **Google Cloud Data Fusion**: Used for processing and transforming data.
4. **Python 3.7+**: Required for running the ETL scripts.

## Process Steps

### 1. Install Apache Airflow

- Install Apache Airflow to orchestrate the ETL pipeline.

### 2. Set up Google Cloud Data Fusion

- Create a Google Cloud Data Fusion instance and configure the pipeline for data processing.

### 3. Set up Airflow DAG

- Place the employee_data_etl.py file in the Airflow dags/ directory and configure it to trigger your Data Fusion pipeline.

### 4. Prepare the Extract Script

- The extract.py script will handle extracting data from the provided employee_data.csv file.

### 5. Sample Input Data

- The employee_data.csv file contains employee details to be processed.

### 6. Airflow Configuration

- Initialize the Airflow database and start the scheduler and web server.

### 7. Trigger the Pipeline

- Trigger the ETL pipeline from the Airflow UI or CLI.

### 8. Monitoring and Logs

- Use the Airflow UI to monitor task statuses and check logs for troubleshooting.
