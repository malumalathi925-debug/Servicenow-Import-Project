Import Data Using Transform Maps (Spreadsheet)

 ServiceNow Micro Project

This project demonstrates how employee data from an Excel spreadsheet can be imported into ServiceNow using Import Sets and Transform Maps.

 Project Overview

The project implements an end-to-end employee data import process in ServiceNow. Spreadsheet data is loaded into an Import Set table and transformed into a custom Employee Test table using a Transform Map.

The project also demonstrates Coalesce to prevent duplicate records and uses Reports and Dashboards to visualize employee information.

Technologies and Features

- ServiceNow
- Import Sets
- Import Set Table
- Transform Maps
- Field Mapping
- Coalesce
- Custom Tables
- Reports
- Dashboards
- Excel Spreadsheet

Project Workflow

Excel Spreadsheet  
↓  
Import Set Table  
↓  
Transform Map  
↓  
Field Mapping  
↓  
Transform Data  
↓  
Employee Test Table  
↓  
Reports  
↓  
Dashboard

 Custom Table

Table: Employee Test  
Name: `u_employee_test`

 Fields
-------------------------------
| Field              | Type   |
-------------------------------
| Employee ID        | String |
| Employee Name      | String |
| Email | String     | String |
| Department         | String |
| Location           | String |

 Import Set

Label: Employee Import  
Name: `u_employee_import`

 Transform Map

**Name:** Sample Spreadsheet Import  
**Source Table:** Employee Import  
**Target Table:** Employee Test

## Coalesce

Employee ID is configured as the Coalesce field to identify existing employee records and prevent duplicate records during repeated imports.

## Reports

The following reports were created:

1. Employees by Department – Pie Chart
2. Employees by Location – Bar Chart
3. Employee List Report – List

## Dashboard

**Dashboard Name:** Employee Analytics Dashboards

The dashboard contains the employee reports and provides a centralized view of employee information.

## Documentation

Detailed step-by-step project documentation is available in:

**Import Data Using Transform Maps.docx**

## Sample Data

The project uses an Excel spreadsheet containing employee information for importing into ServiceNow.

## Conclusion

This project provides practical experience in importing spreadsheet data into ServiceNow, configuring Transform Maps, using Coalesce for duplicate prevention, and creating Reports and Dashboards for employee data analysis.
