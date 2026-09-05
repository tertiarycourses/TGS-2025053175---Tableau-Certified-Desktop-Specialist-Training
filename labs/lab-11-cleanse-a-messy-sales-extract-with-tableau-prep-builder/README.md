# Lab 11 — Cleanse a Messy Sales Extract with Tableau Prep Builder

**Scenario:** Harbourfront Trading exports raw transactions with currency text, inconsistent city spellings, split name fields, duplicate rows and wide monthly budget columns. Analysts need one governed, refreshable clean table before any Tableau Desktop analysis.

**Goal:** Build a repeatable Tableau Prep flow that profiles, cleans, reshapes and outputs an analysis-ready table

**Data:** `Lab-11-Harbourfront-Prep-Cleansing.xlsx` (synthetic mock data)

**Starter Tableau workbook:** `starter.twb`

## Detailed procedure

1. **Open Tableau Prep Builder and connect to Lab-11-Harbourfront-Prep-Cleansing.xlsx.**
   Start with the Q1 Transactions sheet; Q2 and Q3 are brought in and unioned at step 10. Read the Read Me, Data Dictionary and Control sheets first. If cosmetic title rows appear above the header, switch on Use Data Interpreter and confirm the corrected header row.
2. **Add a Clean step and study the profile pane before changing anything.**
   Record which fields show dirty types, nulls, outliers or too many distinct members. The profile, not the data grid, reveals distribution problems.
3. **Repair the Price Paid field so it can become a number.**
   Values contain currency symbols and thousands separators. Create a calculated field such as REPLACE(REPLACE([Price Paid],',',''),'$','') and only then change the type to Decimal Number; converting directly produces nulls.
4. **Apply cleaning operations to the free-text fields.**
   Use Trim Spaces and Remove Extra Spaces on Customer Name; note the difference from Remove All Spaces, which would destroy multi-word names. Use Remove Punctuation where codes carry stray characters.
5. **Split the Customer Name field.**
   Use Automatic Split first, inspect the result, then use a custom split on the space delimiter if the inferred separator is inconsistent. Rename the outputs First Name and Last Name and remove the original field.
6. **Identify and remove duplicate rows.**
   Profile Transaction ID and confirm the distinct count against the Control sheet; exclude the duplicated records and re-check the count.
7. **Filter out invalid records.**
   Exclude rows with null Transaction ID and negative Sales using a calculation or range filter; state in a note how many rows each filter removed and why they are not legitimate data.
8. **Standardise city members using Group and Replace.**
   Apply pronunciation and spelling-similarity matching to merge misspelt city variants, then review every proposed group manually — fuzzy matching can merge genuinely different members.
9. **Pivot the wide monthly budget columns to rows.**
   Add a Pivot step on the Monthly Budget sheet, convert the twelve month columns into Month and Budget Amount fields, and set Month to a date type.
10. **Union the quarterly transaction sheets and merge mismatched fields.**
   Q2 uses Sales Amount while the others use Net Sales; merge them into one field and confirm no avoidable nulls remain. Keep the Table Name provenance field.
11. **Join the Region lookup and add calculated fields.**
   Inner join on Region Code, remove the duplicated key column, then add a Profit calculated field and verify it against the Control sheet.
12. **Reorder a step in the change list to see the effect, then restore it.**
   This proves the flow is an auditable, reorderable pipeline rather than a set of one-off clicks.
13. **Add an Output step and run the flow.**
   Write a .hyper extract or CSV named Lab-11-Clean-Output into this lab folder, then save the flow as Lab-11-Harbourfront-Cleansing.tfl.
14. **Connect Tableau Desktop to the cleaned output.**
   Build one validation worksheet showing record count, distinct customers, total sales and total profit, and reconcile against the Control sheet.

## Acceptance test

The flow runs end to end without errors; Price Paid is numeric, duplicates and invalid rows are removed, city members are standardised, budgets are pivoted long, the union has no avoidable nulls, the join does not multiply rows, and the output reconciles to the Control sheet.

Complete `acceptance-checklist.md` and save evidence in an `evidence/` subfolder.
