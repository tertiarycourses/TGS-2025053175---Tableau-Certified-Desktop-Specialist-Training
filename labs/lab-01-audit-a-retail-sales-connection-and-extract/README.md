# Lab 01 — Audit a Retail Sales Connection and Extract

**Scenario:** Northstar Retail needs a trustworthy weekly sales source before analysts build regional reporting.

**Goal:** Connect to Excel, validate field metadata, compare live and extract behaviour

**Data:** `Lab-01-Northstar-Retail-Orders.xlsx` (synthetic mock data)

**Starter Tableau workbook:** `starter.twb`

## Detailed procedure

1. **Open Tableau Desktop and choose Microsoft Excel.**
   Select Lab-01-Northstar-Retail-Orders.xlsx from this lab folder.
2. **Inspect the Read Me and Data Dictionary worksheets first.**
   Confirm the scenario, expected grain and required fields before using Orders.
3. **Drag Orders to the data canvas and review the preview.**
   One row must represent one order line; compare the preview row count with the Control sheet.
4. **Correct field types.**
   Order Date and Ship Date are dates; Customer ID and Order ID are strings; Sales, Cost and Discount are decimals.
5. **Rename technical fields and add comments.**
   Use business-friendly captions while preserving source meaning.
6. **Assign geographic roles.**
   Set Country/Region, State/Province and City roles; resolve ambiguous locations with country context.
7. **Set default properties.**
   Format Sales, Cost and Profit as SGD; Discount as a percentage; default Profit aggregation as SUM.
8. **Create a worksheet named Connection Check.**
   Show record count, distinct orders, minimum date, maximum date and total sales.
9. **Record the live/extract decision.**
   Use the decision table in the workbook and explain freshness, performance, portability and refresh implications.
10. **Create a Tableau extract.**
   Hide unused audit fields first, then extract all required rows.
11. **Run a full refresh and inspect extract properties.**
   Confirm the data-as-of timestamp and row count remain correct.
12. **Save the workbook as Lab-01-Connection-Audit.twbx.**
   Capture the Connection Check worksheet as evidence.

## Acceptance test

The source has the expected row count and date range, geographic fields are recognised, currency/percentage defaults are correct, and the extract refreshes without errors.

Complete `acceptance-checklist.md` and save evidence in an `evidence/` subfolder.
