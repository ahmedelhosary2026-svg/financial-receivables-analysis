# Project 1: Financial Health & Receivables Optimization

## Overview
This project demonstrates financial acumen and data modeling for Power BI, focusing on Accounts Receivable (AR) analysis. The dataset simulates real AR scenarios, with a significant proportion of overdue invoices to highlight business risk.

## Data Model
- **File:** `financial_ar.csv`
- **Columns:**
  - `client_id`
  - `invoice_id`
  - `invoice_amount`
  - `invoice_date`
  - `due_date`
  - `days_overdue`
  - `risk_segment` (`High`, `Medium`, `Low`)
  - `collection_status` (`Collected`, `Unpaid`, `Partial`)

At least 30% of invoices are overdue by more than 60 days to reflect real-world collection challenges.

## Analysis Logic

### Days Sales Outstanding (DSO)
- **Formula:**  
  DSO = (Total Receivables ÷ Total Credit Sales) × Number of Days in Period

### Collection Efficiency Ratio
- **Formula:**  
  Collection Efficiency = (Total Collected Amount ÷ Total Due Amount) × 100

### Risk Classification Logic
- **Criteria:**  
  - High: `days_overdue > 60` OR `invoice_amount > 2500`
  - Medium: `days_overdue` between 31–60 OR `invoice_amount` between 1000–2500
  - Low: Otherwise

## Usage Instructions
1. Load `financial_ar.csv` into your preferred analytics tool (Excel, Power BI, etc.).
2. Use the provided formulas to calculate DSO and Collection Efficiency.
3. Apply the risk logic to segment clients and invoices for targeted collection strategies.

## Portfolio Skills Validated
- Financial Accounting analysis
- Data modeling for reporting/BI
- Risk segmentation logic