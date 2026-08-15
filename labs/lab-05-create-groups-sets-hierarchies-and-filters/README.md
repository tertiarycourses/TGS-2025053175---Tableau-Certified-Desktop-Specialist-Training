# Lab 05 — Create Groups, Sets, Hierarchies and Filters

**Scenario:** HarbourLife Insurance needs a reusable segmentation view for advisers and portfolio managers.

**Goal:** Organise customer data and apply filters at the intended analytical stage

**Data:** `Lab-05-HarbourLife-Customer-Segmentation.xlsx` (synthetic mock data)

**Starter Tableau workbook:** `starter.twb`

## Detailed procedure

1. **Connect to Lab-05-HarbourLife-Customer-Segmentation.xlsx.**
   Validate policy count, premium and claim totals.
2. **Create a Customer Tier group.**
   Combine micro and small-business codes into Emerging; keep Enterprise and Strategic separate.
3. **Create a Top 20 Customers set by SUM(Annual Premium).**
   Show IN/OUT instead of filtering it away.
4. **Create a High Claims set.**
   Use Claims Paid greater than the threshold documented on the Control sheet.
5. **Create a combined Risk Attention set.**
   Combine Top Customers and High Claims to identify commercially material risk.
6. **Build the Geography hierarchy.**
   Region > Country > City, then test expand/collapse.
7. **Build the Product hierarchy.**
   Product Family > Product Plan.
8. **Add an Active Policy filter.**
   Keep policies active as of the workbook's stated reporting date.
9. **Add a relative Renewal Date filter.**
   Show renewals in the next 90 days.
10. **Make Region a context filter.**
   Observe how it changes the Top 20 set result and explain order of operations.
11. **Create an Adviser Worklist dashboard sheet.**
   Expose only purposeful filters and show set membership.
12. **Save as Lab-05-Segmentation.twbx.**
   Document one case where a group, set and filter would produce different outcomes.

## Acceptance test

The two hierarchies drill correctly, sets produce expected membership, relative dates use the reporting date, and the learner can explain how context changes Top-N evaluation.

Complete `acceptance-checklist.md` and save evidence in an `evidence/` subfolder.
