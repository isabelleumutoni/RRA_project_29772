RRA_project_29772
# Revenue Administration Database

## Overview

A PostgreSQL database project for managing revenue administration data, including taxpayers, tax registrations, declarations, assessments, payments, audits, objections, penalties, and tax types.

## Technologies

* PostgreSQL
* SQL
* psql

## Main Tables

* `taxpayer`
* `tax_registration`
* `tax_type`
* `tax_period`
* `tax_declaration`
* `tax_assessment`
* `tax_payment`
* `tax_objection`
* `tax_audit`
* `audit_finding`
* `tax_officer`
* `tax_centre`
* `penalty`
* `business`
* `property`
* `vehicle`

## SQL Concepts Used

* Primary & Foreign Keys
* `INSERT` and `SELECT`
* `INNER JOIN`
* `LEFT JOIN`
* `RIGHT JOIN`
* `GROUP BY`
* `HAVING`
* `COUNT()` and `SUM()`
* `COALESCE()`

## Project Output

Screenshots of the database tables and SQL query results are shown below.

### Database Tables


all data in tables
```sql
SELECT 'TAXPAYER' AS table_name, COUNT(*) AS record_count FROM TAXPAYER
UNION ALL
SELECT 'TAX_CENTRE', COUNT(*) FROM TAX_CENTRE
UNION ALL
SELECT 'TAX_TYPE', COUNT(*) FROM TAX_TYPE
UNION ALL
SELECT 'TAX_OFFICER', COUNT(*) FROM TAX_OFFICER
UNION ALL
SELECT 'TAX_REGISTRATION', COUNT(*) FROM TAX_REGISTRATION
UNION ALL
SELECT 'TAX_PERIOD', COUNT(*) FROM TAX_PERIOD
UNION ALL
SELECT 'TAX_DECLARATION', COUNT(*) FROM TAX_DECLARATION
UNION ALL
SELECT 'TAX_ASSESSMENT', COUNT(*) FROM TAX_ASSESSMENT
UNION ALL
SELECT 'TAX_PAYMENT', COUNT(*) FROM TAX_PAYMENT
UNION ALL
SELECT 'BANK', COUNT(*) FROM BANK
UNION ALL
SELECT 'PENALTY', COUNT(*) FROM PENALTY
UNION ALL
SELECT 'TAX_AUDIT', COUNT(*) FROM TAX_AUDIT
UNION ALL
SELECT 'AUDIT_FINDING', COUNT(*) FROM AUDIT_FINDING
UNION ALL
SELECT 'TAX_REFUND', COUNT(*) FROM TAX_REFUND
UNION ALL
SELECT 'TAX_OBJECTION', COUNT(*) FROM TAX_OBJECTION
UNION ALL
SELECT 'ENFORCEMENT_CASE', COUNT(*) FROM ENFORCEMENT_CASE
UNION ALL
SELECT 'BUSINESS', COUNT(*) FROM BUSINESS
UNION ALL
SELECT 'PROPERTY', COUNT(*) FROM PROPERTY
UNION ALL
SELECT 'VEHICLE', COUNT(*) FROM VEHICLE
UNION ALL
SELECT 'REVENUE_TARGET', COUNT(*) FROM REVENUE_TARGET
ORDER BY table_name;
```
![Database Tables](screenshoots/data_record.png)

### SQL Query Results

### querry 1
![Query Output 1](screenshoots/query-querry1.png)

![Query Output 2](images/query-output-2.png)

![Query Output 3](images/query-output-3.png)
```

> Replace the image names with the actual names of your screenshots.

## How to Run

```sql
CREATE DATABASE revenue_administration_db;
\c revenue_administration_db
```

Then run the SQL file containing the table creation, data insertion, and queries.

## Author

**[Your Name]**
