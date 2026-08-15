# QA and Alignment Report — v4

Course: Tableau Certified Desktop Specialist Training  
Course code: TGS-2025053175  
QA date: 15 August 2026

## Overall verdict

**PASS.** The generated courseware, lab package and assessment set satisfy the current WSQ build requirements and the user brief. The Google Drive release was dry-run first, uploaded to the verified course folder, read back, and checked for answer-key privacy. LMS/TMS was then updated through a full read-modify-write and independently verified against a protected before-snapshot.

## A. PPT quality audit — PASS

- 151 rendered slides visually inspected as six contact sheets, with changed slides 145 and 151 inspected at full size.
- Separate general and named Dr Alfred Ang trainer-profile slides are present.
- Visual LMS download slide, visual WA → PP assessment-flow slide, and visual practice-exam slide are present.
- Final slide contains the exact Tableau Desktop Specialist practice-exam URL and QR code.
- Cover carries a single `v4` label matching the `-v4` PPTX filename.
- Five editable native PowerPoint charts and 151 Fade transitions are present.
- No off-slide shapes and no explicit click-by-click step headings were detected in the PPTX.
- Detailed procedures remain in the Learner Guide and individual lab READMEs.

## B. Assessment quality audit — PASS

- Original instrument structure preserved: WA (SAQ) + PP, four items each, one hour each.
- Candidate and answer-key papers cover K1–K4 and A1–A4 exactly.
- All questions are open-ended and scenario-based.
- Rendered PDF verifier passes all four documents: cover-only page 1; candidate information, instructions, LMS link and grading on page 2; assessment content from page 3; no prohibited `For Official Use Only` text.
- WA pagination was repaired during QA by adding the required colon to the item headings and then regenerated and reverified.
- Candidate papers are anyone-with-link viewers on Drive; current and archived answer keys have zero `anyone` permissions and require Google sign-in.

### K/A coverage matrix

| Code | Assessment item | Teaching and practice source |
|---|---|---|
| K1 | WA Question 1 | Objective 1.1.3; slide 27; Lab 1 |
| K2 | WA Question 2 | Objective 2.1.6; slide 61; Lab 4 |
| K3 | WA Question 3 | Objectives 1.2.1–1.2.3; slides 32–35; Labs 2 and 10 |
| K4 | WA Question 4 | Objective 4.3.2; slide 136; Lab 10 |
| A1 | PP Task 1 | Relationship/model validation; Labs 2 and 10; slides 32–35 and 137–138 |
| A2 | PP Task 2 | Crosstab and percent-of-total table calculation; Labs 4, 6 and 10; slides 64, 76, 81, 85 and 137 |
| A3 | PP Task 3 | Dynamic sets; Labs 5 and 10; slides 68, 83 and 137 |
| A4 | PP Task 4 | Scatterplot and trend model; Labs 4 and 10; slides 58, 81 and 137 |

## C. Lesson Plan — PASS

- WSQ cover, version-control record and generated TOC are present.
- Day 1 and Day 2 each total 480 minutes excluding lunch.
- Final deck slide map was consumed after the practice-exam additions; activity and assessment slide references match the 151-slide deck.
- DOCX and current rendered PDF are present.

## D. Learner Guide — PASS

- WSQ cover, version-control record and generated TOC are present.
- 44 rendered pages; cover, version/TOC and sampled lab pages were inspected visually.
- All 10 labs have detailed click-by-click instructions; 53 explicit `Step` headings were detected in the PDF.
- Current house skill keeps the Learner Guide as DOCX/PDF only, so no divergent Markdown mirror is retained.

## E. Labs and alignment — PASS

- 10 individual lab folders, each containing one realistic Excel workbook, `README.md`, `starter.twb` and `acceptance-checklist.md`.
- Every lab has 12–15 detailed procedure steps and an explicit acceptance test.
- All 10 Tableau starter workbooks are well-formed XML.
- All 10 Excel workbooks recalculated successfully in LibreOffice with zero formula errors.
- Dataset scale ranges from 648 to 2,920 primary fact rows, with mixed-grain supporting tables, dictionaries and control sheets where relevant.
- Drive `Activities/` readback: 41 files = 10 XLSX + 10 TWB + 10 checklists + 11 READMEs.

## F. Files, versions and distribution — PASS

- PPTX/PDF, Learner Guide DOCX/PDF and Lesson Plan DOCX/PDF are present under `courseware/`.
- Confidential `assessment/`, `.env`, references, build tools, assets and QA renders are excluded from the public GitHub release.
- `COURSEWARE_LINK` is stored in the ignored root `.env`.
- Superseded Drive files were moved to per-folder `archive/` locations rather than deleted.
- Drive link readback identified the current trainer slide, learner slide, LG, LP, two candidate papers and Activities folder.
- LMS/TMS production update resolved the exact course record and wrote all seven learner-facing URLs: trainer slides, learner slides, LG, LP, Labs, WA and PP.
- Post-write verification passed for the flat URL fields and nested assessment methods; answer keys were withheld, the unused practical method was disabled, all unrelated course fields were unchanged, and the mode-600 snapshot was deleted on success.

## Source preservation

The 688-slide legacy deck was treated as the coverage floor. Its useful Tableau Desktop concepts were retained and reorganised against the official four-domain blueprint. Repetitive click sequences were moved to the Learner Guide and labs so the PPT remains visual and concept-led. See `SOURCE-COVERAGE-v4.md` for the detailed mapping.
