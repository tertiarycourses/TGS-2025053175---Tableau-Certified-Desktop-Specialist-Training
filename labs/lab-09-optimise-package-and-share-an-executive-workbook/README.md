# Lab 09 — Optimise, Package and Share an Executive Workbook

**Scenario:** Sentinel Energy must brief executives while giving analysts a governed interactive workbook.

**Goal:** Create device layouts, a story, exports and a governed sharing plan

**Data:** `Lab-09-Sentinel-Energy-Executive-Sharing.xlsx` (synthetic mock data)

**Starter Tableau workbook:** `starter.twb`

## Detailed procedure

1. **Connect to Lab-09-Sentinel-Energy-Executive-Sharing.xlsx.**
   Review Energy Performance and Governance Notes.
2. **Build the Executive Performance dashboard.**
   Show demand, cost, renewable share and outage risk.
3. **Apply the presentation style guide.**
   Use accessible colours, readable type, consistent numbers and concise legends.
4. **Configure viz animations.**
   Use subtle animation for a year or scenario change and verify the final state remains understandable.
5. **Create a phone layout.**
   Reorder to KPI > key trend > exception list; remove nonessential views.
6. **Test multiple device previews.**
   Confirm legibility, touch targets and no horizontal scrolling.
7. **Create a story with three points.**
   Situation, evidence and recommended action; give every point a decision-oriented caption.
8. **Save a .twb and inspect dependencies.**
   Explain why a recipient without the source may see broken connections.
9. **Save a .twbx.**
   Confirm the Excel data is packaged and compare file size.
10. **Export PDF, PNG and PowerPoint.**
   Record which interaction and freshness capabilities are lost.
11. **Draft a Server/Cloud publish plan.**
   Specify project, permissions, refresh schedule, owner and certification status.
12. **Audit underlying-data exposure.**
   Test View Data and export permissions against the Governance Notes.
13. **Save as Lab-09-Executive-Sharing.twbx.**
   Submit both layouts, story, exports and the sharing decision table.

## Acceptance test

Desktop and phone layouts are usable, the story has three coherent points, TWBX is portable, static exports are labelled with data-as-of context, and the publish plan protects underlying data.

Complete `acceptance-checklist.md` and save evidence in an `evidence/` subfolder.
