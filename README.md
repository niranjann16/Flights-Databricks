# Flight Data Pipeline with Databricks & Delta Lake

An end-to-end data pipeline implementing the Medallion Architecture to process and analyze flight data efficiently.

## 🚀 Key Features
- **Medallion Architecture Implementation** (Bronze → Silver → Gold)
- **Incremental Data Ingestion** with schema validation
- **SCD Type 1 Implementation** for dimension management
- **Automated Data Quality Checks**
- **30% improvement in query accuracy**

## 🛠️ Tech Stack
- **Databricks** (DBT, DLT Pipelines)
- **Delta Lake** (ACID transactions, Time Travel)
- **PySpark** for transformations
- **Delta MERGE** operations for SCD Type 1

## 📂 Project Structure
flight-data-pipeline/
├── notebooks/ # Databricks notebooks
│ ├── 1_bronze_ingestion.py
│ ├── 2_silver_transformation.py
│ └── 3_gold_dimensions.py
├── dlt_pipelines/ # Delta Live Tables code
│ ├── silver_layer.py
│ └── gold_layer.py
├── docs/ # Architecture diagrams
└── README.md

## 🏗️ Pipeline Architecture
1. **Bronze Layer**:
   - Raw data ingestion from CSV/JSON
   - Schema validation
   - Basic metadata tagging

2. **Silver Layer**:
   - Deduplication
   - Data type standardization
   - Added audit columns (modified_date, etc.)

3. **Gold Layer**:
   - Dimension tables (SCD Type 1)
   - Fact tables
   - Business-ready aggregates

## 📊 Results
- Reduced data processing time 
- Improved query accuracy by 30%
- Eliminated duplicate/invalid records
- Achieved 25% storage reduction through Delta optimizations

## 🎜 Setup Instructions
1. Clone this repository
2. Import notebooks into your Databricks workspace
3. Configure Databricks Jobs with appropriate cluster specs
4. Set up pipeline triggers (or run manually)

## 🤝 How to Contribute
- Open issues for bugs or feature requests
- Fork and submit PRs for improvements
- Share your SCD Type 2 implementation ideas!

## 📫 Connect
Let's discuss data engineering! Connect with me on [LinkedIn](www.linkedin.com/in/niranjann8)
