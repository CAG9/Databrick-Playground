# Databrick Playground
This repository is a hands-on tutorial archive designed to help users learn, implement, and master core concepts and code execution on the Databricks platform. It serves as a comprehensive knowledge base with reproducible notebooks for self-paced learning.
# Project Description
This project implements a complete data ingestion and transformation using Databricks and the Medallion Architecture (Bronze → Silver → Gold).
The workflow is designed to ensure data quality, scalability, and clear separation between raw ingestion, cleaned data, and business-ready datasets.

* Architecture Overview
Catalog Creation:
A dedicated Databricks catalog was created to organize the project’s data assets.

Three Schemas (Layers):

Bronze: Raw ingested data with minimal processing.

Silver: Cleaned and standardized data, with transformations applied to improve quality.

Gold: Curated, business-ready datasets for analytics and reporting.

* Data Ingestion

Data is ingested into the Bronze layer by creating  databrick tables.

* Data Transformation & Cleaning

To promote data quality and consistency across layers, the following steps were applied:

Handling missing values: Replacement, imputation, or filtering as needed.

Data type corrections: Casting columns to their appropriate types.

Standardizing formats: Normalizing date, numeric, and categorical fields.

Deduplication: Removing duplicated records to ensure data integrity.

Column renaming: Creating clear and consistent column names across layers.

Filtering invalid records: Removing rows with corrupted or invalid data.

Feature engineering: Adding derived columns required for downstream analysis.

Schema enforcement: Ensuring datasets adhere to predefined structures for reliability.

Each transformation step builds upon the previous layer, ensuring that by the time the data reaches Gold, it is optimized for analytics, BI dashboards, and machine learning workflows.
## Author
- Cesar Arcos-Gonzalez: cesar99ag@gmail.com
## License
MIT License
## Tools and Technologies
- Pyspark
- Databricks
- SQL
