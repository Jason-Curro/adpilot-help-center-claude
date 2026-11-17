---
id: "csv-errors"
title: "Fix CSV import errors"
description: "Diagnose common CSV file rejection messages."
category: "troubleshooting"
feature: "troubleshooting"
audience: "merchant"
difficulty: "beginner"
language: "en"
plans: ["PRO"]
keywords: ["csv", "error", "missing column", "encoding", "file"]
last_reviewed: "2026-11-17"
translation_id: "csv-errors"
related: ["csv-requirements", "upload-csv"]
---

# Fix CSV import errors

## Quick checks
If the Optimizer rejects your report, first check the file format in [CSV format and required columns](../optimizer/csv-requirements.md). The exact error message can help identify the cause.

| Message or symptom | What to check |
| --- | --- |
| No file selected | Select a CSV before submitting. |
| Must be `.csv` | Export CSV, not `.xlsx` or a renamed spreadsheet. |
| Too small / empty | Export a report with actual data rows; minimum 1 KiB. |
| Too large | Reduce the date range; maximum 10 MiB. |
| Unsupported encoding | Re-export or save as UTF-8, not UTF-16. |
| Unsupported delimiter | Use comma or semicolon. |
| Missing columns | Compare report headers with the 13 required data categories. |
| Too many rows / columns | Maximum 50,000 data rows and 200 columns. |
| No valid rows | Verify the report contains usable data, not just a header. |
| Not a valid text CSV | Export a clean CSV directly from Meta Ads Manager. |

## If the import succeeds but figures look wrong
1. Compare total spend and purchases in AdPilot with the same period in Meta Ads Manager.
2. Re-export **one campaign per file**, with simple numeric formatting and without thousands separators.
3. Ensure that **purchase value** is not a ROAS column and that interest/audience values are genuine.
4. If the numbers still differ, do **not** act on the recommendations; ask AdPilot support to review the format without posting your private report publicly.

## Recommended recovery
1. Re-export the original report using the required columns.
2. Open it in a text editor only if necessary to check encoding and delimiters.
3. Upload again **once** after correcting the issue.
4. If the same message persists, note it for support rather than sharing the raw file in chat.

For the step-by-step import workflow, read [Upload a CSV to the Optimizer](../optimizer/upload-csv.md).
