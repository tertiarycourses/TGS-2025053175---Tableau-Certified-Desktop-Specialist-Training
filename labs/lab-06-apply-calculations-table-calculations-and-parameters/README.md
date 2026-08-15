# Lab 06 — Apply Calculations, Table Calculations and Parameters

**Scenario:** Crescent Hospitality wants profitability, occupancy and performance trends with user-controlled thresholds.

**Goal:** Create reliable row-level, aggregate and view-dependent analytics

**Data:** `Lab-06-Crescent-Hospitality-Analytics.xlsx` (synthetic mock data)

**Starter Tableau workbook:** `starter.twb`

## Detailed procedure

1. **Connect to Lab-06-Crescent-Hospitality-Analytics.xlsx.**
   Use the Daily Performance sheet and inspect KPI definitions.
2. **Create Gross Profit.**
   SUM([Room Revenue]) + SUM([F&B Revenue]) - SUM([Operating Cost]).
3. **Create Occupancy Rate.**
   SUM([Rooms Sold]) / SUM([Rooms Available]); format as percentage.
4. **Create RevPAR.**
   SUM([Room Revenue]) / SUM([Rooms Available]); verify its aggregation grain.
5. **Create Performance Band.**
   Use an IF/ELSEIF rule based on Occupancy Rate and Gross Profit.
6. **Build a monthly running revenue total.**
   Set Compute Using to Month and partition by Hotel.
7. **Build each hotel's percent of regional revenue.**
   Validate addressing and partitioning after rearranging the view.
8. **Add a 3-month moving average.**
   Explain the null edge at the start of each partition.
9. **Create a KPI Selector parameter.**
   Allow Room Revenue, Gross Profit, Occupancy and RevPAR.
10. **Create a Selected KPI calculation.**
   Return the chosen measure with consistent aggregation.
11. **Add a parameter-driven target reference line.**
   Use a separate numeric Target parameter.
12. **Display totals and audit them.**
   Explain why averaging daily percentages differs from a ratio of summed numerators/denominators.
13. **Save as Lab-06-Advanced-Analytics.twbx.**
   Capture the parameter states and table-calculation settings.

## Acceptance test

Calculations match the Control sheet, table calculations keep intended addressing/partitioning, parameters affect the view, and totals use mathematically valid logic.

Complete `acceptance-checklist.md` and save evidence in an `evidence/` subfolder.
