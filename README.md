# 🚀 Azure Data Engineering Pipeline  
### *(ADF + Azure Data Lake + Databricks Lakehouse)*

---


## 🏷️ Badges

![Azure](https://img.shields.io/badge/Azure-0078D4?style=for-the-badge&logo=microsoftazure&logoColor=white)
![Databricks](https://img.shields.io/badge/Databricks-FF3621?style=for-the-badge&logo=databricks&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![PySpark](https://img.shields.io/badge/PySpark-FDEE21?style=for-the-badge&logo=apachespark&logoColor=black)
![Delta Lake](https://img.shields.io/badge/Delta_Lake-003366?style=for-the-badge&logo=databricks&logoColor=white)
![ADF](https://img.shields.io/badge/Azure_Data_Factory-0078D4?style=for-the-badge&logo=microsoftazure&logoColor=white)

---

## 📌 Project Overview

### 🧩 Problem Statement
Design and implement a **scalable end-to-end data pipeline** that:
- Ingests raw data  
- Processes it through structured layers  
- Produces analytics-ready datasets  

---

### 📊 Dataset Description

| Entity     | Description |
|------------|------------|
| Customers  | User demographics & contact info |
| Products   | Product details, pricing, branding |
| Orders     | Transactional sales data |
| Regions    | Geographic mapping |

---

## 🏗️ Architecture

```
📂 Source (ADLS Gen2)
        ↓
⚙️ Azure Data Factory (ADF)
        ↓
🥉 Bronze Layer (Raw Data)
        ↓
🔥 Databricks (Processing)
        ↓
🥈 Silver Layer (Cleaned Data)
        ↓
🥇 Gold Layer (Business Tables)
        ↓
📊 BI / Analytics Output
```

---

## ⚙️ ADF Implementation

### 🔹 Key Components

| Component | Purpose |
|----------|--------|
| Copy Activity | Moves data to Data Lake |
| Trigger | Automates execution |
| Pipeline | Orchestrates workflow |

---

## 🔥 Databricks Implementation

### 💻 Cluster Setup
- Configured compute cluster  
- Optimized for PySpark workloads  

### 📓 Notebooks

| Layer   | Notebooks |
|--------|----------|
| Bronze | Bronze_Layer |
| Silver | Orders, Customers, Products, Regions |
| Gold   | Customers, Products, Orders |

---

## 🔄 Data Transformation

### 🥉 Bronze
- Raw ingestion  
- No transformation  

### 🥈 Silver
- Data cleaning  
- Null handling  
- Filtering & grouping  

### 🥇 Gold
- Fact & Dimension tables  
- Star schema  
- Optimized queries  

---

## 📊 Results / Output

### 📌 Final Tables

| Table Name   | Type |
|-------------|------|
| DimCustomers | Dimension |
| DimProducts  | Dimension |
| FactOrders   | Fact |

---

## ⚠️ Challenges & Solutions

| Problem | Solution |
|--------|--------|
| Connection issues | Configured Entra ID |
| Duplicate data | Used MERGE (upsert) |
| Schema mismatch | Cleaned in Silver layer |
| Pipeline errors | Implemented DAG dependencies |

---

## 🎯 Conclusion

### ✅ Key Learnings
- Built **Lakehouse architecture**
- Hands-on with:
  - Azure Data Factory  
  - Azure Data Lake  
  - Databricks  
- Implemented:
  - Medallion Architecture  
  - Delta Lake  
  - SCD Type 2  

---

## 🌟 Final Outcome
✔ Raw data → Structured → Analytics-ready  
✔ Fully automated pipeline  
✔ Ready for dashboards & BI tools  

---

## 📎 Author
**Hamza Rizwan**  
Data Science Student | Data Engineering Enthusiast
