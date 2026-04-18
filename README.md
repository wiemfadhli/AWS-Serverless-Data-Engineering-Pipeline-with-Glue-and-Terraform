# 🚀 Cloud Data Pipeline Project  
### 🪣 AWS S3 Data Lake → AWS Glue ETL → Data Quality Framework (Terraform)

---

## 📌 Project Overview

This project implements a **scalable cloud-based data engineering pipeline** using AWS services and Infrastructure as Code (**Terraform**).

It is designed around a **modern AWS Data Lake architecture using Amazon S3**, where data flows through multiple processing layers:

> **Raw Data → ETL Processing → Data Validation → Trusted Dataset**

The goal is to simulate a **production-grade data engineering system** using cloud-native tools.

---

## 🏗️ Architecture

The pipeline follows a **Medallion Data Lake Architecture (Bronze / Silver / Gold)**:

```text
🪣 Amazon S3 Data Lake
        ↓
📥 Bronze Layer (Raw Data)
        ↓
🔄 AWS Glue ETL Job (Transformation)
        ↓
📦 Silver Layer (Processed Data)
        ↓
🧪 AWS Glue Data Validation Job
        ↓
🏆 Gold Layer (Trusted / Analytics Ready)
## 🪣 Data Lake (Amazon S3)

Amazon S3 is used as a **central Data Lake storage system**, storing all raw and processed data in a scalable cloud architecture.

---

### 📁 Data Lake Structure

```text
s3://data-lake-bucket/
│
├── raw/         # 🥉 Bronze Layer → Raw ingested data
├── processed/   # 🥈 Silver Layer → Cleaned & transformed data
└── trusted/     # 🥇 Gold Layer → Final validated dataset






