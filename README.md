📌 Project Overview

This project implements a scalable, production-style data engineering pipeline on AWS using Infrastructure as Code (Terraform).

It demonstrates how raw data can be ingested, transformed, and validated in a fully automated cloud environment using modern data engineering practices.

🏗️ Architecture

The pipeline follows a layered data flow approach:

Raw Data (Amazon S3)
        ↓
AWS Glue ETL Job (Data Cleaning & Transformation)
        ↓
Processed Data (Amazon S3)
        ↓
AWS Glue Data Quality Job (Validation Layer)
        ↓
Trusted / Analytics-Ready Dataset
⚙️ Core Capabilities

✔ Automated data ingestion into S3 (Data Lake)
✔ Data cleaning and transformation using AWS Glue (PySpark)
✔ Feature engineering (e.g., company age calculation)
✔ Schema standardization and data normalization
✔ Data validation and quality checks
✔ Fully automated infrastructure provisioning using Terraform

📊 Dataset Description

The dataset contains structured information about organizations, including:

Organization ID
Name
Website
Country
Industry
Founded Year
Number of Employees
Description
🔄 ETL Process

The transformation layer includes:

Standardization of column names (snake_case format)
Removal of duplicates and null values
Data type casting (numeric and string normalization)
Feature engineering: company_age = current_year - founded_year
🧪 Data Quality Validation

The validation layer ensures:

✔ Dataset completeness
✔ Schema consistency
✔ Required field validation
✔ Post-transformation data integrity

🧰 Technology Stack
AWS S3 – Data Lake storage layer
AWS Glue (PySpark) – ETL processing engine
AWS IAM – Secure access management
Terraform – Infrastructure as Code (IaC)
Python – Data transformation logic
🚀 Business Value

This pipeline simulates real-world enterprise data systems and provides:

Reliable and automated data processing
Scalable cloud-based architecture
Improved data quality and trust
Reduced manual ETL operations
Production-ready infrastructure design
👨‍💻 Author

Designed and implemented as a Cloud Data Engineering project focusing on AWS, ETL pipelines, and Infrastructure automation using Terraform.
