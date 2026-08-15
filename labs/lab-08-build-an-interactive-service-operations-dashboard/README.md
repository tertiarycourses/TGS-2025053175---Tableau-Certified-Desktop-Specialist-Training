# Lab 08 — Build an Interactive Service Operations Dashboard

**Scenario:** ApexCare's service director needs a daily dashboard for backlog, SLA risk, channel demand and team performance.

**Goal:** Compose worksheets, containers, filters, tooltips and dashboard actions

**Data:** `Lab-08-ApexCare-Service-Operations.xlsx` (synthetic mock data)

**Starter Tableau workbook:** `starter.twb`

## Detailed procedure

1. **Connect to Lab-08-ApexCare-Service-Operations.xlsx.**
   Review Tickets, Agents, SLA Targets and Control sheets.
2. **Create the four KPI calculations.**
   Open Backlog, SLA Breach Rate, Median Resolution Hours and CSAT.
3. **Build Backlog by Team as a bar chart.**
   Sort descending and use an SLA-risk highlight.
4. **Build Daily Ticket Trend as a line chart.**
   Show Opened and Resolved tickets with consistent units.
5. **Build Channel × Priority as a highlight table.**
   Use count on text and colour.
6. **Build Resolution vs CSAT as a scatterplot.**
   Use Agent on Detail and Team on Colour.
7. **Create a fixed 1366×768 dashboard.**
   Use tiled vertical and horizontal containers to establish hierarchy.
8. **Place KPI tiles and views.**
   Keep the main decision view prominent and align padding consistently.
9. **Add Date, Team and Priority filters.**
   Apply each only to relevant worksheets.
10. **Add a Team filter action.**
   Selecting a team bar filters the trend, matrix and scatterplot.
11. **Add a Priority highlight action.**
   Hovering the matrix highlights related marks without removing context.
12. **Rewrite tooltips.**
   Lead with the business meaning, then the key values and filter context.
13. **Test dashboard states.**
   Use the acceptance checklist for default, selected, cleared and no-data states.
14. **Save as Lab-08-Service-Dashboard.twbx.**
   Export dashboard PNG and action settings screenshots.

## Acceptance test

The dashboard loads in the target size, KPIs match Control, filters are scoped, actions clear correctly, no object overlaps, and a manager can answer the three stated operational questions.

Complete `acceptance-checklist.md` and save evidence in an `evidence/` subfolder.
