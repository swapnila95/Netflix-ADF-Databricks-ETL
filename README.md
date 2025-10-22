# Netflix-ADF-Databricks-ETL
Netflix Azure End-to-End Data Engineering Project
##**Overview**

This project demonstrates a scalable, cloud-based data engineering solution built using Azure Data Factory, Databricks, Delta Live Tables (DLT), and Azure Data Lake Storage Gen2. Following the Medallion architecture (Bronze, Silver, Gold layers), the pipeline ingests raw Netflix datasets from GitHub, transforms and aggregates data using PySpark and DLT, and enables advanced analytics and reporting. The project is based on this YouTube walkthrough, which details every step from data ingestion to reporting.

##**Architecture**
Data Ingestion (Bronze Layer):
Azure Data Factory (ADF) pipelines pull raw CSV files from GitHub into Azure Data Lake Storage (ADLS Gen2) using dynamic, parameterized pipelines for scalable automation.

Data Transformation (Silver Layer):
Databricks notebooks and PySpark scripts process, clean, and enrich the ingested data. Databricks Autoloader is used for incremental ETL.

Data Aggregation (Gold Layer):
Delta Live Tables (DLT) automate further aggregation and star schema transformation, enabling analytics-ready datasets for BI tools.

Reporting & Visualization:
Data is made available for Azure Synapse and Power BI for reporting and dashboard creation.

Repository Structure
Folder	Description
/ADF	Azure Data Factory pipelines, datasets, linked services
/Databricks	Notebooks, PySpark scripts, Delta Live Table ETL workflows
/RawData_AND_Notebooks	Source data and sample notebooks
/Docs	Project documentation and architecture diagrams
Step-by-Step Usage
Clone this repository.

Configure ADF:

Connect your ADF workspace to the /ADF folder.

Import pipelines and linked services, set up credentials, and run ingestion jobs to pull data from GitHub into ADLS Gen2.

Run Databricks Notebooks:

Open the /Databricks folder in your Databricks workspace Repos.

Follow each notebook for incremental ingestion, transformation, workflow orchestration, and Delta Live Tables setup.

Validate results and explore outputs.

Use built-in notebook validations.

Visualize results using Power BI or Synapse Analytics as applicable.

References
Project walkthrough YouTube video

Original Dataset and Notebooks

[Azure Data Factory Documentation]​

[Databricks Documentation]​

[Delta Live Tables Guide]​


