# Azure End-to-End Data Engineering Project

> End-to-End Azure Data Engineering Pipeline using Azure Data Factory, ADLS Gen2, Azure Databricks, Azure Synapse Analytics and Power BI.

## Project Overview

This project demonstrates an end-to-end Azure Data Engineering solution following the Medallion Architecture (Bronze → Silver → Gold).

## Architecture

```text
GitHub CSV Files
      │
      ▼
Azure Data Factory
      │
      ▼
Bronze (ADLS Gen2)
      │
      ▼
Azure Databricks (PySpark)
      │
      ▼
Silver (ADLS Gen2)
      │
      ▼
Azure Synapse Analytics
      │
      ▼
Gold Layer
      │
      ▼
Power BI Dashboard
```

## Technology Stack

- Azure Data Factory
- Azure Data Lake Storage Gen2
- Azure Databricks
- PySpark
- Azure Synapse Analytics
- SQL
- Power BI
- GitHub

## Repository Structure

```text
datasets/
notebooks/
sql/
screenshots/
architecture/
README.md
LICENSE
.gitignore
requirements.txt
```

## Pipeline Flow

1. GitHub CSV datasets
2. ADF ingestion
3. Bronze Layer
4. Databricks transformations
5. Silver Layer
6. Synapse SQL
7. Gold Layer
8. Power BI Dashboard

## Screenshots

Use your numbered screenshots in the `screenshots` folder.

## Challenges Solved

- Databricks deployment
- Service Principal authentication
- RBAC permissions
- ADLS authorization
- Synapse integration

## Author

**Karthik**  
Data Engineer  
Bangalore, India

GitHub: https://github.com/DigitalKarthikAI
