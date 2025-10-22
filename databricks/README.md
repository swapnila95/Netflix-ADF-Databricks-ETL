Databricks Folder - Netflix Azure Data Engineering Project


**Overview**

This folder contains Databricks notebooks and related scripts for building an end-to-end data engineering pipeline in Azure. It demonstrates incremental data loads, dynamic notebook parameterization, PySpark transformations, orchestration with Databricks Workflows, and Delta Live Tables aligned with the Medallion architecture.

**Prerequisites**

Databricks workspace (Azure)

Access to project datasets (see RawData_AND_Notebooks)

Linked Azure Data Lake and ADF resources

**Step-by-Step Instructions**

**1. Import Notebooks**

Download required notebooks and scripts from this folder, or use the provided DBC/ IPYNB files.

In Databricks, click Workspace > Repos and import these notebooks into your Git-synced folder.​

**2. Setup Data Lake Connections**

Validate connections to Azure Data Lake and configure mount points as shown in the notebooks or as per your workspace.

**3. Incremental Ingestion Using Autoloader**

Open the notebook for incremental loading.

Set parameters for the source path and schema location.

Configure and run Databricks Autoloader for efficient incremental data file ingestion.

**4. Data Transformation with PySpark**

Run the PySpark transformation notebook on the ingested raw/bronze data.

Apply cleaning, joining, and enrichment steps as outlined.

Output processed data to silver and gold containers in Lake.

**5. Orchestrate with Workflows**

Use Databricks Jobs to automate pipeline runs (parameterized and scheduled).

Configure workflow activities (for each, conditional, etc.) as demonstrated in the notebooks.

**6. Delta Live Tables for Gold Layer**

Open the notebook for Delta Live Tables.

Define gold layer tables and transformations.

Deploy Delta Live Table pipelines for managed ETL orchestration.

**7. Validation and Output**

Use assertion and test cells in notebooks to validate output quality.

Store or export results for downstream analytics.

References
Project video walkthrough

Original Dataset Repo

Azure Databricks Documentation


