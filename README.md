# Commodity Closing — T-SQL

Microsoft SQL Server twin of the Databricks notebook
[commodity-closing-simulation](https://github.com/YzrSalih/commodity-closing-simulation).

Same question, different engine: what cleared this month, at what average price, and do buys and sells balance?

## What this repo shows

- Excel is the source file an accounting user would drop in.
- T-SQL loads those rows, checks them, and builds the monthly close inside SQL Server.
- A stored procedure is the close. You run it. You do not paste a query every month.
- VBA is the button that sends the sheet in and writes the summary back.

## Stack

- SQL Server Express
- SSMS
- T-SQL: tables, inserts, stored procedures
- Excel + VBA

Not in this repo: Access, SAP, Databricks.

## Run order

1. Install SQL Server Express and SSMS.
2. In SSMS, connect to `localhost\SQLEXPRESS`.
3. Execute `sql/01_schema_and_seed.sql`.
4. Later, in order: data-quality check, monthly close procedure, reconciliation, Excel + VBA.

## Author

Salih Yazar
