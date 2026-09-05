<div align="center">

# 📊 Tableau Desktop Foundations

**Connect, clean, analyse and share data with Tableau Desktop and Tableau Prep Builder — in two hands-on days.**

[![Register](https://img.shields.io/badge/📝_Register-Enrol_Now-1F6FEB?style=for-the-badge)](https://www.tertiarycourses.com.sg/wsq-tableau-certified-desktop-specialist-training.html)
[![WSQ Funded](https://img.shields.io/badge/WSQ-SkillsFuture_Funded-10B981?style=for-the-badge)](https://www.tertiarycourses.com.sg/wsq-tableau-certified-desktop-specialist-training.html)

![Course Code](https://img.shields.io/badge/Course_Code-TGS--2025053175-555B66)
![Duration](https://img.shields.io/badge/Duration-2_Days_·_16_Hours-7C3AED)
![Level](https://img.shields.io/badge/Level-Beginner-10B981)
![TSC](https://img.shields.io/badge/TSC-Data_Analytics_·_ATP--PIN--2001--1.1-1F6FEB)
![Labs](https://img.shields.io/badge/Labs-11_Hands--On-F59E0B)
![Assessment](https://img.shields.io/badge/Assessment-WA_(SAQ)_+_PP-555B66)

**[📝 Register for this course →](https://www.tertiarycourses.com.sg/wsq-tableau-certified-desktop-specialist-training.html)**

</div>

---

## About This Course

Tableau Desktop Foundations takes you from a raw, messy spreadsheet to a governed, interactive dashboard. You will connect to real data sources, repair and reshape dirty data in **Tableau Prep Builder**, model it correctly with relationships and joins, build the core chart portfolio, and package the result as a dashboard other people can trust and act on.

The course is built for analysts, executives and business users who work with spreadsheets today and want a reliable, repeatable way to answer questions with data — no prior Tableau experience required. Content is aligned to the official Tableau Desktop Specialist exam blueprint, so the course also doubles as structured preparation for that credential.

## Learning Outcomes

| # | Outcome |
|---|---|
| **LO1** | Identify and connect appropriate data sources, then prepare trustworthy Tableau data models. |
| **LO2** | Organise fields and create effective visual elements that answer business questions. |
| **LO3** | Extract, combine and analyse data using relationships, joins, unions, filters and calculations. |
| **LO4** | Build, format and share interactive dashboards and workbooks that communicate meaningful insights. |

## Course Topics & Labs

Each lab lives in its own folder under [`labs/`](labs/) with a realistic synthetic dataset, a Tableau starter workbook, a step-by-step `README.md` and an acceptance checklist.

| Topic | Weight | Covers | Labs |
|---|---:|---|---|
| **1. Connecting to and Preparing Data in Tableau Desktop** | 23% | Live vs extract, metadata, relationships, joins, unions, field properties, **data cleansing with Tableau Prep Builder** | [01](labs/lab-01-audit-a-retail-sales-connection-and-extract/), [02](labs/lab-02-model-orders-returns-products-and-targets/), [03](labs/lab-03-union-monthly-files-and-join-store-attributes/), [11](labs/lab-11-cleanse-a-messy-sales-extract-with-tableau-prep-builder/) |
| **2. Exploring and Analyzing Data in Tableau Desktop** | 37% | Charts, groups, sets, hierarchies, filters, analytics, calculations, parameters | [04](labs/lab-04-build-the-core-tableau-chart-portfolio/), [05](labs/lab-05-create-groups-sets-hierarchies-and-filters/), [06](labs/lab-06-apply-calculations-table-calculations-and-parameters/), [07](labs/lab-07-analyse-southeast-asia-logistics-geographically/) |
| **3. Sharing Insights with Dashboards and Workbooks** | 25% | Formatting, dashboards, actions, device layouts, stories, export, publish | [08](labs/lab-08-build-an-interactive-service-operations-dashboard/), [09](labs/lab-09-optimise-package-and-share-an-executive-workbook/) |
| **4. Understanding Tableau Concepts and Certification Preparation** | 15% | Dimensions vs measures, discrete vs continuous, aggregation, exam strategy | [10](labs/lab-10-capstone-northstar-retail-executive-workbook/) + all-domain review |

### Featured: Lab 11 — Data Cleansing with Tableau Prep Builder

Lab 11 hands you a deliberately messy sales extract and asks you to make it analysis-ready:

| Defect in the data | What you learn to fix it |
|---|---|
| `Price Paid` is text like `$1,577.30` and refuses to become a number | Strip currency symbols and separators with a calculation, *then* change the type |
| Cities recorded as `Singapore`, `Singapor`, `SINGAPORE`, `Singapore.` | **Group and Replace** with pronunciation and spelling matching |
| Duplicate rows, null keys and negative sales | Profile the key, then filter from the profile pane |
| `Customer Name` holds first and last name in one field | Automatic and custom **Split** |
| Q2 calls the measure `Sales Amount`, other quarters `Net Sales` | **Union**, then merge the mismatched fields |
| Budgets sit in twelve wide month columns | **Pivot** columns to rows |

A `Control` sheet states the expected counts, so you can prove the cleaned output reconciles.

## Tools

| Tool | Purpose |
|---|---|
| [Tableau Desktop](https://www.tableau.com/products/desktop) | Connect, analyse, visualise and build dashboards |
| [Tableau Prep Builder](https://www.tableau.com/products/prep/download) | Profile, clean, reshape and output data as a repeatable flow |
| Microsoft Excel | Source data for every lab |

| Practice & Reference | Link |
|---|---|
| Tableau Desktop Specialist practice exam | [exams.tertiaryinfotech.com](https://exams.tertiaryinfotech.com/practice-exams/tableau/tableau-desktop-specialist) |
| Official exam guide | [Salesforce Certification](https://help.salesforce.com/s/articleView?id=005298988&type=1&language=en_US) |
| Free official Tableau training | [tableau.com/learn/training](https://www.tableau.com/learn/training) |
| Course materials (learners) | [lms-tms.tertiaryinfotech.com](https://lms-tms.tertiaryinfotech.com/) |

## Repository Structure

```
.
├── courseware/                 # Generated, learner-facing artifacts
│   ├── Tableau Desktop Foundations-v5.pptx / .pdf
│   ├── LG-Tableau Desktop Foundations.docx / .pdf     # Learner Guide
│   └── LP-Tableau Desktop Foundations.docx / .pdf     # Lesson Plan
├── labs/                       # 11 self-contained labs
│   └── lab-NN-<slug>/
│       ├── README.md                   # Step-by-step procedure
│       ├── Lab-NN-<Scenario>.xlsx      # Synthetic dataset
│       ├── starter.twb                 # Tableau starter workbook
│       └── acceptance-checklist.md     # Evidence and quality gate
├── QA-ALIGNMENT-v5.md          # QA and alignment record
├── SOURCE-COVERAGE-v5.md       # Source-to-topic mapping
└── README.md
```

> **Note:** the confidential `assessment/` folder (question papers and trainer-only answer keys) and the `reference/` source material are **not** published in this repository. Assessments are distributed to trainers via Google Drive and the LMS.

## Course Details

| | |
|---|---|
| **Course Title** | Tableau Desktop Foundations |
| **Course Code** | TGS-2025053175 |
| **TSC** | Data Analytics · ATP-PIN-2001-1.1 |
| **Duration** | 2 days · 16 hours (including 2-hour assessment) |
| **Level** | Beginner — no prior Tableau experience required |
| **Assessment** | Written Assessment (WA/SAQ) — 4 open-ended questions, 1 hour, open book<br>Practical Performance (PP) — 4 Tableau tasks, 1 hour, open book |
| **Mode** | Instructor-led concept teaching, demonstrations and hands-on Tableau labs |
| **Certification** | WSQ Statement of Attainment; aligned to the Tableau Desktop Specialist exam |
| **Provider** | Tertiary Infotech Academy Pte Ltd · UEN 201200696W |

### Funding

This course is **WSQ SkillsFuture funded**. Learners need at least **75% attendance** and a **Competent** assessment outcome to qualify for funding. For current subsidy rates and eligibility, see the [course registration page](https://www.tertiarycourses.com.sg/wsq-tableau-certified-desktop-specialist-training.html).

## Building the Courseware

All artifacts are generated from a single source of truth, so the slides, Lesson Plan, Learner Guide and labs never drift apart.

```bash
# Regenerate everything (slides, LP, LG, labs and PDFs)
bash courseware/build/build_courseware.sh

# Regenerate just the labs
python3 courseware/build/generate_labs.py

# Regenerate the assessment set (trainer-only; not published here)
python3 courseware/build/build_assessments.py
```

> The build sources under `courseware/build/` are excluded from this public repository.

## Data and Privacy

All lab records are deterministic synthetic mock data created for learning. They do not describe real people, customers or organisations. Do not substitute confidential workplace data when publishing to Tableau Public.

## Contact

| | |
|---|---|
| 🌐 **Course page** | [Tableau Desktop Foundations](https://www.tertiarycourses.com.sg/wsq-tableau-certified-desktop-specialist-training.html) |
| ✉️ **Email** | [training@tertiaryinfotech.com](mailto:training@tertiaryinfotech.com) |
| ☎️ **Tel** | +65 6255 5547 |
| 🎓 **LMS / TMS** | [lms-tms.tertiaryinfotech.com](https://lms-tms.tertiaryinfotech.com/) |

---

<div align="center">

### Ready to turn messy data into decisions?

**[📝 Register for Tableau Desktop Foundations →](https://www.tertiarycourses.com.sg/wsq-tableau-certified-desktop-specialist-training.html)**

© 2026 Tertiary Infotech Academy Pte Ltd · UEN 201200696W

</div>
