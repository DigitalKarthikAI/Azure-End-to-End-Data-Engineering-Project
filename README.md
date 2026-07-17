# 🚀 Azure End-to-End Data Engineering Project

> **An end-to-end Azure Data Engineering pipeline built using Azure Data Factory, Azure Data Lake Storage Gen2, Azure Databricks (PySpark), Azure Synapse Analytics, and Power BI following the Medallion Architecture.**

<p align="center">
<img src="architecture/architecture.png" width="100%">
</p>

---

# 📌 Business Problem

Organizations receive raw transactional data from multiple operational systems. Raw data is often inconsistent, duplicated, and not optimized for analytics.

This project demonstrates how to build a modern Azure Data Engineering pipeline that ingests raw CSV files, transforms them into trusted datasets, creates an analytical Gold layer, and visualizes insights through Power BI.

---

# 🏗️ Solution Architecture

GitHub CSV → Azure Data Factory → ADLS Gen2 (Bronze) → Azure Databricks (Silver) → Azure Synapse (Gold) → Power BI

---

# 🛠️ Technology Stack

| Service | Purpose |
|---------|---------|
| Azure Data Factory | Data Ingestion |
| Azure Data Lake Storage Gen2 | Data Lake |
| Azure Databricks | PySpark Transformations |
| Azure Synapse Analytics | SQL Analytics |
| Power BI | Visualization |
| GitHub | Source Data |

---

# 📂 Repository Structure

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

---

# ⭐ Key Features

- End-to-End Azure Data Pipeline
- Medallion Architecture (Bronze → Silver → Gold)
- PySpark Data Transformation
- Synapse SQL Gold Layer
- Interactive Power BI Dashboard
- Modular Repository Structure

---

# 🔄 Pipeline Flow

1. GitHub stores AdventureWorks datasets.
2. Azure Data Factory ingests data.
3. Files land in the Bronze layer.
4. Databricks cleans and transforms data into Silver.
5. Synapse creates analytical Gold views.
6. Power BI consumes Gold datasets.

---

# 📸 Project Walkthrough

<details>
<summary><b>1. Azure Resource Setup</b></summary>

Resource Group used to organize all Azure resources.

![](screenshots/01-resource-group.png)

Azure Storage Account hosting the data lake.

![](screenshots/02-storage-account.png)

Bronze, Silver and Gold containers.

![](screenshots/03-storage-containers.png)

</details>

<details>
<summary><b>2. Azure Data Factory</b></summary>

ADF workspace overview.

![](screenshots/04-adf-home.png)

Pipeline that copies GitHub CSV files into ADLS Bronze.

![](screenshots/05-adf-pipeline.png)

Linked services connecting Azure resources.

![](screenshots/06-adf-linked-service.png)

</details>

<details>
<summary><b>3. Azure Databricks</b></summary>

Workspace configuration.

![](screenshots/07-databricks-workspace.png)

PySpark notebook implementing Bronze → Silver transformations.

![](screenshots/08-databricks-notebook.png)

Compute cluster used to execute transformations.

![](screenshots/09-databricks-compute.png)

</details>

<details>
<summary><b>4. Azure Synapse Analytics</b></summary>

Synapse workspace.

![](screenshots/10-Synapse-home.png)

SQL development environment.

![](screenshots/11-Synapse-develop.png)

SQL objects used to expose Gold views.

![](screenshots/12-Synapse-datatab.png)

</details>

<details>
<summary><b>5. Data Lake Layers</b></summary>

Bronze Layer (Raw)

![](screenshots/13-Bronze-container.png)

Silver Layer (Cleaned)

![](screenshots/14-Silver-container.png)

Gold Layer (Analytics Ready)

![](screenshots/15-Gold-container.png)

</details>

<details>
<summary><b>6. Power BI Dashboard</b></summary>

Interactive dashboard built on the Gold layer.

![](screenshots/16-Powerbi-dashboard.png)

</details>

---

# 🚧 Challenges & Solutions

| Challenge | Solution |
|-----------|----------|
| ADLS authentication | Configured Service Principal & RBAC |
| Databricks storage access | OAuth configuration |
| Bronze → Silver transformation | Implemented using PySpark |
| Gold layer | Created Synapse SQL views |
| Secret scanning during Git push | Removed client secret before publishing |

---

# 📊 Project Summary

- Azure Services Used: **6**
- Data Layers: **3**
- Databricks Notebook: **1**
- Synapse SQL Scripts: **Included**
- Power BI Dashboard: **1**
- Architecture: **Medallion**

---

# 📚 Key Learnings

- Azure Data Factory Pipelines
- Azure Data Lake Storage Gen2
- Azure Databricks with PySpark
- Medallion Architecture
- Azure Synapse Analytics
- Power BI Reporting
- Git & GitHub Portfolio Management

---

# 🚀 Future Enhancements

- CI/CD with GitHub Actions
- Terraform Infrastructure as Code
- Incremental Data Loads
- Data Quality Validation
- Monitoring & Alerting

---

# 👨‍💻 Author

**Karthik**  
**Data Engineer**  
Bangalore, India

GitHub: https://github.com/DigitalKarthikAI

If you found this project useful, consider giving it a ⭐.
