# QA and Alignment Report — v5

Course: Tableau Desktop Foundations
Course code: TGS-2025053175
QA date: 5 September 2026

## Scope of this revision

v5 retitles the course and extends Topic 1 with data cleansing in Tableau Prep Builder.

| Change | Detail |
|---|---|
| Course title | `Tableau Certified Desktop Specialist Training` → `Tableau Desktop Foundations`. The certification name "Tableau Desktop Specialist" is retained wherever it refers to the exam or credential. |
| Topic titles | Topic 1 Connecting to and Preparing Data in Tableau Desktop · Topic 2 Exploring and Analyzing Data in Tableau Desktop · Topic 3 Sharing Insights with Dashboards and Workbooks · Topic 4 Understanding Tableau Concepts and Certification Preparation. |
| Topic 1 content | New fourth section "Cleanse data with Tableau Prep Builder" with ten objectives 1.4.1–1.4.10, sourced from `reference/Data Cleansing with TABLEAU PREP (Full Notes) - Dr Alvin Ang.pptx`. |
| Labs | New Lab 11 "Cleanse a Messy Sales Extract with Tableau Prep Builder" under Topic 1, with a purpose-built dirty dataset. Labs 1–10 keep their numbering. |
| Assessment | WA question K1 and PP task A1 rewritten to assess Tableau Prep cleansing. Instrument structure unchanged: WA (SAQ) + PP, four items each, one hour each. |
| Version | v4 → v5; superseded artifacts moved to `courseware/archive/` and `assessment/archive/`. |

## A. Deck — 165 slides

- Cover shows a single `v5` label matching the `-v5` PPTX filename, with the new course title.
- Page footer now derives from the course title rather than a hardcoded certification string.
- Topic 1 runs slides 19–63 and now includes the ten Tableau Prep objective slides in the house four-tile format.
- Lab 11 overview and acceptance slides are at 61–63; `slide_map.json` records `lab11: 61`.
- Slide map: topic1 19 · topic2 64 · topic3 104 · topic4 133 · wrap 154 · practice exam 165.

## B. Lesson Plan

- Day 1 was rebalanced to accommodate Lab 11 across the pre-lunch and post-lunch blocks.
- Day 1 and Day 2 each total 480 instructional minutes excluding lunch, 9:00am–6:00pm, with contiguous session times and no gaps.
- Version-control record carries the v5 row.

## C. Learner Guide

- 49 rendered pages with generated TOC (40 entries).
- Carries the ten new Topic 1 objectives 1.4.1–1.4.10 and the full Lab 11 procedure.
- Version-control record carries the v5 row.
- Lab data filenames are now read from the labs generator's single `SCENARIOS` source rather than a duplicated map, removing a drift risk.

## D. Lab 11 dataset

The Lab 11 workbook carries deliberate, documented defects so the cleansing steps have something real to fix:

| Defect | Where |
|---|---|
| Currency text with `$` and thousands separators blocking numeric conversion | `Price Paid` |
| Misspelt and inconsistently cased city variants | `City` |
| Duplicate rows (18), null keys (12) and negative sales (15) | Q1–Q3 Transactions |
| Mismatched union field name (`Sales Amount` vs `Net Sales`) | Q2 Transactions |
| Concatenated first and last name requiring a split | `Customer Name` |
| Wide twelve-column month layout requiring a pivot | Monthly Budget |

A `Control` sheet states the expected counts so learners can reconcile the cleaned output.

## E. Distribution

- Confidential `assessment/`, `reference/`, build tools, assets and `.env` remain excluded from the public GitHub release.
- Superseded versions are archived rather than deleted.

## Source preservation

The 688-slide legacy deck remains the coverage floor for Topics 1–4. The 321-slide Tableau Prep reference deck is the source for the new Topic 1 cleansing section and Lab 11; its click-by-click sequences were condensed into concept-led objective slides, with the procedural detail placed in the Learner Guide and the Lab 11 README. See `SOURCE-COVERAGE-v5.md` for the detailed mapping.
