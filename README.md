# Contoso Retail Data Warehouse (SSIS ETL Project)
## Project Overview
![SSIS ETL Pipeline](assets/Project.png)
This project is an end-to-end Data Engineering solution built using SQL Server Integration Services (SSIS) and SQL Server Data Warehouse concepts.
It simulates a real-world enterprise retail analytics system designed to transform raw operational data into a structured, analytics-ready data warehouse.
The solution is based on a Star Schema dimensional model, optimized for fast querying and business intelligence reporting.

## Architecture Overview
![SSIS ETL Pipeline](assets/Architicture.png)
The system follows a standard ETL pipeline:
Source Systems → SSIS ETL Pipeline → SQL Server Data Warehouse → Data Marts → BI Reporting Layer

Data Warehouse Design (Star Schema)
The data warehouse is designed using a dimensional modeling approach (Kimball methodology).
Fact Table

FactSales
Transaction-level data
Measures: Sales Amount, Quantity, Revenue, Returns

Dimension Tables
DimProduct
DimCustomer
DimStore
DimCategory

The schema is designed to reduce complexity in queries and improve analytical performance.

## ETL Process (SSIS)
The ETL pipeline was developed using SSIS and includes the following stages:
Extract
Data extracted from operational source systems
Transform

Data cleaning and standardization
Handling missing values and inconsistencies

Business rule implementation
Surrogate key generation

Data validation and integrity checks

Load
Dimensions loaded first
Fact table loaded after ensuring referential integrity

Data Marts
To support business intelligence and reporting, multiple data marts were created:

ProductSalesPerMonth
SalesPerStore
CustomerSalesAndReturn

These are optimized for analytical queries and BI tools such as Power BI.

## Technologies Used
SQL Server
SSIS (SQL Server Integration Services)
SQL Server Data Warehouse
T-SQL
Dimensional Modeling (Star Schema)

## Key Concepts Applied :
Data Warehouse Design
Star Schema Architecture
ETL Pipeline Development
Fact and Dimension Modeling
Data Cleaning and Transformation
Surrogate Key Management
BI-Ready Data Modeling

## Project Goals

Transform raw transactional data into structured analytics data

Design a scalable and maintainable data warehouse

Enable fast and efficient reporting for business intelligence

Simulate real-world enterprise data engineering workflow



