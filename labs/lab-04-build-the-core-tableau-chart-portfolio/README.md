# Lab 04 — Build the Core Tableau Chart Portfolio

**Scenario:** A consumer-electronics team needs views for ranking, trend, relationship, geography, composition and precise lookup.

**Goal:** Create and justify nine chart patterns from one realistic sales dataset

**Data:** `Lab-04-Orion-Electronics-Chart-Portfolio.xlsx` (synthetic mock data)

**Starter Tableau workbook:** `starter.twb`

## Detailed procedure

1. **Connect to Lab-04-Orion-Electronics-Chart-Portfolio.xlsx.**
   Use the Orders sheet and validate the Control totals.
2. **Build Sales by Category as a sorted bar chart.**
   Use length on a common baseline and meaningful labels.
3. **Build Monthly Sales and Profit as a line view.**
   Use a continuous Month date and annotate one material change.
4. **Build Discount vs Profit Ratio as a scatterplot.**
   Place Product on Detail and Category on Colour; identify clusters and outliers.
5. **Build Sales by City as a symbol map.**
   Use Sales on Size and Profit Ratio on Colour; fix any ambiguous geography.
6. **Build Sales and Cost on a combined axis.**
   Use Measure Names/Values only because both measures share SGD units.
7. **Build Sales vs Profit as a dual-axis view.**
   Use bars and a line, synchronise only if units and interpretation support it.
8. **Build Category Mix as stacked bars.**
   Limit colours and compare both total and composition.
9. **Build Order Density by Store Coordinates.**
   Use generated Latitude/Longitude or supplied coordinates and explain smoothing.
10. **Build Region × Category as a highlight table.**
   Show exact Sales text with a sequential colour scale.
11. **Complete the Chart Choice worksheet.**
   For each view state the business question, visual encoding and one limitation.
12. **Save as Lab-04-Chart-Portfolio.twbx.**
   Export a contact sheet or screenshots of all nine views.

## Acceptance test

All nine chart types are present, each matches its stated question, axes and units are honest, maps resolve locations, and each view has a concise evidence-based insight.

Complete `acceptance-checklist.md` and save evidence in an `evidence/` subfolder.
