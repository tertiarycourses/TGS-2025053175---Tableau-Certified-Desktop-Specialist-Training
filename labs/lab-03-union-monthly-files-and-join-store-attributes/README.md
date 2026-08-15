# Lab 03 — Union Monthly Files and Join Store Attributes

**Scenario:** MetroMart receives separate monthly transaction tabs plus a store master and needs one analysis-ready source.

**Goal:** Append compatible tables, merge mismatched fields and join a lookup

**Data:** `Lab-03-MetroMart-Union-and-Join.xlsx` (synthetic mock data)

**Starter Tableau workbook:** `starter.twb`

## Detailed procedure

1. **Connect to Lab-03-MetroMart-Union-and-Join.xlsx.**
   Review the January, February and March sheet structures.
2. **Create a manual union of the three monthly sheets.**
   Confirm Tableau adds Table Name and Sheet provenance fields.
3. **Inspect null-heavy columns caused by a deliberate field-name mismatch.**
   February uses Sales Amount while other months use Net Sales.
4. **Merge mismatched fields.**
   Create one Net Sales field and verify February values are no longer null.
5. **Add the Stores sheet in the physical layer.**
   Left join on Store ID so all transactions remain.
6. **Validate the join.**
   Compare pre/post row counts and count unmatched Store IDs.
7. **Rename provenance fields.**
   Use Source Month and Source Sheet labels.
8. **Create aliases for store formats.**
   Display EXPRESS as Express and SUPERCENTER as Supercentre.
9. **Set default number and date formats.**
   Net Sales and Gross Profit are SGD; Transaction Date uses dd mmm yyyy.
10. **Build Monthly Union QA.**
   Show monthly records, sales and unmatched-store counts.
11. **Save the reusable data source.**
   Create a .tds or .tdsx and state what is packaged.
12. **Save as Lab-03-Union-Join.twbx.**
   Capture the data-source canvas and QA view.

## Acceptance test

All three months appear, merged sales has no avoidable nulls, record counts match Control, the left join preserves transactions, and the saved source opens with metadata intact.

Complete `acceptance-checklist.md` and save evidence in an `evidence/` subfolder.
