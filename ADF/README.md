Azure Data Factory (ADF) Pipelines


**Overview**

This folder contains the Azure Data Factory (ADF) pipelines, datasets, linked services, and configuration files used in the Netflix Azure Data Engineering Project. The pipelines orchestrate end-to-end ETL workflows, ingesting and transforming raw datasets from multiple sources (including GitHub and Azure Data Lake), with dynamic parameterization and robust data validation.

Project Features
Dynamic and parameterized data ingestion pipelines

Incremental loading and data validation

Integration with Azure Data Lake and Databricks

Modular linked services and datasets

Production-ready template for cloud-scale ETL

Folder Structure
**/pipelines** – JSON files defining ADF pipelines

**/datasets** – JSON files for datasets used in ingestion and transformation

**/linkedServices** – JSON files for connections to Azure resources

**/dataflows** – Optional: Data flow transformations

**/triggers** – Optional: Pipeline scheduling triggers

How To Use
Clone the repository and connect your ADF workspace to the ADF folder.

Import linked services, datasets, and pipelines using the ADF UI or ARM templates.

Configure authentication and connection strings in the linked services files as needed.

Deploy, monitor, and validate your data pipelines.

Documentation
Full documentation and setup instructions are available in the main project README.

Refer to the Azure Data Factory docs for advanced usage and tips:
**https://learn.microsoft.com/en-us/azure/data-factory/**

License
This project is licensed under the MIT License.


