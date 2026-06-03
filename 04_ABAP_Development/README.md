# SAP ABAP: Customer Accounts Receivable Reporting System

> Final Project | ERP Business Application Development | Spring 2024  
> Developed in SAP S/4HANA using ABAP and ALV Grid Display

## Overview

Built two custom ABAP programs to extract, join, and display financial 
data from SAP's core FI/SD tables — solving a real business need: 
giving accounting teams fast, filterable visibility into cleared 
customer invoices without relying on standard transaction reports.

## Business Problem Addressed

Standard SAP A/R reports lack flexible filtering by both company code 
and customer range simultaneously. These programs fill that gap by 
pulling cleared items from BSAD joined with customer master data 
from KNA1, surfacing actionable financial data in ALV format.

## Technical Implementation

| Program | Transaction | Purpose |
|---|---|---|
| Z_245_1306 | Program 01 | A/R cleared items report — filterable by company code & customer range, ALV output |
| Z_245_1307 | Program 02 | Customer-level detail report — shows debit/credit line items with G/L account and clearing document |
| Z1_245_1307 | Program 03 | Accounts Payable cleared items — vendor-level report with posting key indicators |

**Key SAP Tables Used:**
- `KNA1` — Customer Master (general data: name, address, country)
- `BSAD` — A/R Cleared Items (document number, clearing date, amount)
- `LFA1` / `BSAK` — Vendor Master & A/P Cleared Items (Program 03)

**ABAP Concepts Applied:**
- SELECT with JOIN across FI and SD tables
- SELECT-OPTIONS for dynamic range filtering
- ALV Grid (REUSE_ALV_GRID_DISPLAY) for interactive output
- Internal tables and field catalog configuration

## Sample Output

Program 01 retrieves all cleared A/R documents for company US00,  
displaying customer number, name, document number, posting date,  
debit/credit indicator, and clearing document in ALV format.

Program 02 drills into individual customer accounts (e.g., Customer 5997 
— Beantown Bikes, Boston) showing matched debit/credit pairs confirming 
full invoice clearance.

## Skills Demonstrated

`SAP ABAP` `ALV Reporting` `FI Module` `SD Module` `Table Joins` 
`Accounts Receivable` `Financial Reporting` `ERP Customization`
