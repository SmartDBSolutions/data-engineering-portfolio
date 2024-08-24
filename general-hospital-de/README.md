## General Hospital Patient End-To-End Pipeline in Azure

An Azure Data Engineering Project



![General Hospital](https://github.com/SmartDBSolutions/data-engineering-portfolio/blob/ec64868e55a984590a4887c2fbc43844d18a7fec/general-hospital-de/images/hospital.jpg)

## A Brief Introduction to General Hospital Schema

**Patients**: Formula 1 cars are cutting-edge, single-seat racing machines with advanced aerodynamics and powerful engines. They are designed for maximum speed and agility.

**Encounters**: F1 races take place on a variety of tracks, including purpose-built circuits and temporary street circuits in cities around the world.

**OrdersProcedures**: Multiple teams, each with two drivers, compete in the championship. Prominent teams include Mercedes, Ferrari, Red Bull Racing, and McLaren.

## What is Data Engineering

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

- Dominant Patient Encounter dates

- Dominant Teams

- Create PowerBI Dashboards

### Scheduling Requirements



## Solution Architecture

This section should list any major frameworks/libraries used to bootstrap your project. Leave any add-ons/plugins for the acknowledgements section. Here are a few examples.

1. Data Files, Source Database or API

2. Azure Data Factory: ADF is the ETL tool used for data ingestion. I connected the ADF to the SQL server to copy the required tables to the cloud.

3. Azure Data Lake Gen 2: This is where all the data are stored.

4. Azure Databricks: Azure Databricks transformed the data into the required format.

5. Azure Synapse Analytics: This tool will load the Azure SQL database data into the cloud datawarehouse

6. Power BI: To load data from Azure Synapse Analytics and Create reports for business use cases.

7. Azure Active Directory and Azure Key Vault: To enhance security access to the different data in the cloud.



To achieve this, we'll leverage a powerful combination of Azure services:

Azure Data Factory (ADF):
Our data movement workhorse, ADFseamlessly extracts data from the on-premise database.

Azure Key Vault:
The guardian of secrets, Key Vault securely storessensitive information like passwords.

Azure Synapse Analytics (Synapse):
Our cloud-based datawarehouse, optimized for querying and analyzing the transformeddata.

Power BI:
The king of data visualization, Power BI lets us createinteractive reports and dashboards to gain insights from the data.

Setting the Stage:
The first step is creating the necessary resources within Azure. We'll utilizea
Resource Group
to logically group all the services needed for this

This is the conductor of our data pipeline,orchestrating the data movement process.
Azure Data Lake Storage Gen2 (ADLS Gen2):

This serves as ourlanding zone in the cloud, a highly scalable storage solution for theraw data.

Azure Synapse Workspace:
This workspace provides a unifiedenvironment for interacting with Synapse Analytics.


![Architecture Diagram](https://github.com/SmartDBSolutions/data-engineering-portfolio/blob/91c72cfd4406114a3bf326259af5d1aa00d5d797/general-hospital-de/documentation/architecture%20diagram.svg)


### Visualizations

