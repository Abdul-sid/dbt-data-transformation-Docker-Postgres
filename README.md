# 📊 Data Transformation via dbt in PostgreSQL Databases (Dockerized)

# 🌟 Project Overview
This project demonstrates an end-to-end data transformation pipeline using dbt in PostgreSQL databases within a Docker container environment. The process involves extracting data from a source Postgres database, loading it into intermediary SQL files, and transforming the data using dbt to generate meaningful insights in the destination database.

By leveraging Docker for containerized databases and dbt for transformation, this project highlights a scalable approach to handling data transformation tasks.

# Key Highlights:
Extract: Pulled data from the source Postgres database.
Transform: Applied transformations using dbt, cleaning and restructuring the data for analysis in the destination Postgres database.
Load: Loaded the raw data into intermediary SQL files.

# 🛠️ Tools & Technologies
SQL: Used for querying and managing data within the PostgreSQL databases.
Docker: Managed isolated PostgreSQL databases in containers for both source and destination databases.
Postgres: Relational database used as both the source and target for data.
dbt: Transformed and modeled data across different layers.
Python: Script to Automate database connection and dumping in and loading data from sql.

# 📚 Key Skills
Database Management with Docker: Setup and managed PostgreSQL databases in a containerized Docker environment.
Data Transformation: Utilized dbt to apply transformations, cleaning raw data and preparing it for analysis.
SQL Optimization: Implemented efficient SQL queries for data extraction and loading.
Container Orchestration: Leveraged Docker to create an isolated environment for development and testing.
PostgreSQL Expertise: Deepened understanding of PostgreSQL for both OLTP and OLAP use cases.

# 🚀 Project Structure
1. Architecture
Docker Environment: Two PostgreSQL databases (source and destination) running in separate Docker containers.
ELT Process: The dbt tool is used to extract data from the source, load it into intermediary SQL tables, and transform the data into the destination database.
Source DB: Raw data hosted in the first PostgreSQL container.
Destination DB: Transformed data stored in the second PostgreSQL container.
2. ELT Breakdown
Extract: Pulled data from the source Postgres database.
Load: Saved intermediary SQL tables for analysis.
Transform: Leveraged dbt to apply transformations and clean data before loading into the destination Postgres database.

# 📂 Folder Structure (Main folders and files)
``` bash
├── custom_postgres                         # dbt project
│   ├── dbt_project.yml                     # dbt project configuration
│   ├── macros                              # macros for dbt
│   ├── models/example                      # dbt models
│   ├──   ├── All Models and .yml files
├── source_db_init
│   ├── init.sql                            # SQL file for intermediary data storage
├── elt
│   ├── Dockerfile                          # Dockerfile to set up ELT Script
│   ├── elt_script.py                       # Python ELT Script
├── logs
│   ├── dbt.log                             # dbt logs
├── docker-compose.yml                      # Docker-Compose setup for source and destination databases
```
