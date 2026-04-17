========================================
🚀 CLOUD DATA PIPELINE PROJECT
S3 → AWS GLUE ETL → DATA QUALITY FRAMEWORK
========================================

📌 PROJECT OVERVIEW
----------------------------------------
This project implements a scalable AWS-based data engineering pipeline
using Infrastructure as Code (Terraform).

It processes raw data from S3, transforms it using AWS Glue (PySpark),
and validates output using a data quality layer.

----------------------------------------
🏗️ ARCHITECTURE
----------------------------------------

RAW DATA (S3)
      ↓
AWS GLUE ETL JOB
  - Data Cleaning
  - Standardization
  - Feature Engineering
      ↓
PROCESSED DATA (S3)
      ↓
AWS GLUE VALIDATION JOB
  - Data Quality Checks
  - Schema Validation
      ↓
FINAL TRUSTED DATASET

----------------------------------------
📊 DATASET
----------------------------------------
- Organization ID
- Name
- Website
- Country
- Industry
- Founded Year
- Number of Employees
- Description

----------------------------------------
🔄 ETL PROCESS
----------------------------------------
✔ Clean column names (snake_case)
✔ Remove duplicates
✔ Handle null values
✔ Type casting (numeric + string)
✔ Feature engineering:
    company_age = current_year - founded_year

----------------------------------------
🧪 DATA QUALITY CHECKS
----------------------------------------
✔ Validate schema consistency
✔ Check missing values
✔ Ensure non-empty dataset
✔ Verify transformation integrity

----------------------------------------
⚙️ TECHNOLOGIES USED
----------------------------------------
- AWS S3 (Data Lake)
- AWS Glue (ETL - PySpark)
- AWS IAM (Security)
- Terraform (Infrastructure as Code)
- Python (Data Processing)

----------------------------------------
🚀 PURPOSE
----------------------------------------
This project demonstrates real-world data engineering practices:
- Cloud ETL pipeline design
- Data lake architecture
- Infrastructure automation
- Data quality assurance

========================================
