# Lab 02 — Model Orders, Returns, Products and Targets

**Scenario:** GreenBasket Grocers wants sales, returns and monthly targets analysed without duplicating measures across different table grains.

**Goal:** Create relationships and compare them with physical joins

**Data:** `Lab-02-GreenBasket-Data-Model.xlsx` (synthetic mock data)

**Starter Tableau workbook:** `starter.twb`

## Detailed procedure

1. **Connect to Lab-02-GreenBasket-Data-Model.xlsx.**
   Read the Data Dictionary and Grain Audit sheets before modelling.
2. **Place Orders as the root logical table.**
   Confirm one row represents one order line.
3. **Relate Returns to Orders on Order ID and Line ID.**
   Use many-to-one or many-to-many only after checking the supplied uniqueness tests.
4. **Relate Products to Orders on Product ID.**
   Products should be one row per Product ID.
5. **Relate Targets using Month Start and Region.**
   Targets are monthly-region grain, not order-line grain.
6. **Review performance options.**
   State cardinality and referential integrity only when supported by evidence.
7. **Build a Model Validation worksheet.**
   Show Sales, Return Count and Target by Region without flattening the model.
8. **Check unmatched keys.**
   Use the Unmatched Keys sheet to identify intentional and erroneous exceptions.
9. **Create a duplicate copy of the data source for a join experiment.**
   Join Orders to Returns in the physical layer and note the resulting row count.
10. **Compare relationship and join totals.**
   Explain why table grain and join type can change Sales and Return totals.
11. **Document the chosen model.**
   Add a caption that states each table grain and relationship key.
12. **Save as Lab-02-Relationship-Model.twbx.**
   Export the model canvas and validation worksheet screenshots.

## Acceptance test

Sales matches the control total, Return Count matches the Returns table, targets do not duplicate, and the learner can explain why relationships are safer for the mixed-grain model.

Complete `acceptance-checklist.md` and save evidence in an `evidence/` subfolder.
