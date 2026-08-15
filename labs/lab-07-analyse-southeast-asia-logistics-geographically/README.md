# Lab 07 — Analyse Southeast Asia Logistics Geographically

**Scenario:** Meridian Logistics wants to compare shipment volume, delay rates and port congestion across Southeast Asia.

**Goal:** Create symbol, filled and density maps with trustworthy geographic context

**Data:** `Lab-07-Meridian-SEA-Logistics.xlsx` (synthetic mock data)

**Starter Tableau workbook:** `starter.twb`

## Detailed procedure

1. **Connect to Lab-07-Meridian-SEA-Logistics.xlsx.**
   Review Shipments and Location Reference sheets.
2. **Assign geographic roles.**
   Country, State/Province and City must resolve within Southeast Asia.
3. **Use supplied Latitude/Longitude for ports where geocoding is ambiguous.**
   Treat them as geographic measures.
4. **Build Port Shipment Volume as a symbol map.**
   Use Shipment Count on Size and Delay Rate on Colour.
5. **Build Country On-Time Performance as a filled map.**
   Use a diverging scale centred on the target.
6. **Build Congestion Hotspots as a density map.**
   Weight by Delayed Shipments and state the smoothing implication.
7. **Create a Port Type shape map.**
   Use a small distinguishable shape set and keep a legend.
8. **Add informative tooltips.**
   Show Port, Country, Shipments, On-Time %, Avg Delay Hours and reporting period.
9. **Resolve unknown locations.**
   Use Edit Locations and document the correction.
10. **Create a ranked bar alternative.**
   Compare accuracy and purpose with the filled map.
11. **Write one spatial insight and one limitation.**
   Base both on visible evidence.
12. **Save as Lab-07-Geographic-Analysis.twbx.**
   Export all maps and the bar comparison.

## Acceptance test

Locations resolve correctly, map types match the questions, tooltips carry operational context, colour scales are meaningful, and the learner can state when the bar chart is preferable.

Complete `acceptance-checklist.md` and save evidence in an `evidence/` subfolder.
