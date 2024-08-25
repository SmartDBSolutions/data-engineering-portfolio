## General Hospital Patient End-To-End Pipeline in Azure

An Azure Data Engineering Project



![General Hospital](https://github.com/SmartDBSolutions/data-engineering-portfolio/blob/ec64868e55a984590a4887c2fbc43844d18a7fec/general-hospital-de/images/hospital.jpg)

## A Brief Introduction to General Hospital Schema

**Patients**: This file contains patient related data such as patient address and demographic information.

**Encounters**: This file contains the encounter related data for a patient interaction between healthcare provider and patient, such as admission datetime, and provider information.

**OrdersProcedures**: This file contains details about the orders related to a 

## What is Data Engineering

Data engineering is the process of designing and building systems that let people collect and analyze raw data from multiple sources and formats.  Azure is Microsoft's cloud offering and contains a number of services for Data Ingestion, Storage, Transformation, and Serving (Power BI)


## Project Requirements

### Data Ingestion 

- Ingested Data from CSV.

- Ingested Data must have the data columns.

- Ingested data must be in the Parquet Format.

- Analyse the ingested data via Python and SQL

### Data Transformation

- Join key information required to report anything.

- Transformed Data must be stored in column format.

### Analysis Requirements

- Patient Encounter dates

- Most in-demand providers

- Create PowerBI Dashboards

### Scheduling Requirements

TBD

## Solution Architecture

This solutions uses Azure Data Platform services to fulfill the requirements.

1. Data Files, Source Database or API

2. Resource Group - All the services used in the solutions are created and grouped together logically for lifecycle maintenance.

3. Azure Data Factory: ADF is the ETL tool used for data ingestion. Our data movement workhorse, ADF seamlessly extracts data from the on-premise database.I connected the ADF to the SQL server to copy the required tables to the cloud.  

4. Azure Data Lake Gen 2: This is where all the data are stored.  A highly scalable storage solution for the raw (bronze layer), processed (silver layer) and ready for loading (gold).

5. Azure Databricks: Azure Databricks transforms the data into the required formats.

6. Azure Synapse Analytics: This tool will load the Azure SQL database data into the cloud data warehouse.  Synapse Analytics is a cloud-based data warehouse that is optimized for querying and analyzing the transformed data.  The Azure Synapse Workspace provides a unified environment for interacting with Synapse Analytics.

7. Power BI: To load data from Azure Synapse Analytics and Create reports for business use cases.  Power BI lets us create interactive reports and dashboards to gain insights from the data.

8. Azure Active Directory and Azure Key Vault: To enhance security access to the different data in the cloud.  The Key Vault securely stores sensitive information like passwords and keys.


![Architecture Diagram](https://github.com/SmartDBSolutions/data-engineering-portfolio/blob/91c72cfd4406114a3bf326259af5d1aa00d5d797/general-hospital-de/documentation/architecture%20diagram.svg)


### Visualizations and Dashboard
Coming soon!

