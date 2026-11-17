---
id: "csv-requirements"
title: "CSV format and required columns"
description: "Accepted size, encoding, separators and required report fields."
category: "optimizer"
feature: "optimizer"
audience: "merchant"
difficulty: "beginner"
language: "en"
plans: ["PRO"]
keywords: ["csv", "utf8", "semicolon", "columns", "headers", "limit"]
last_reviewed: "2026-11-17"
translation_id: "csv-requirements"
related: ["csv-errors"]
---

# CSV format and required columns

## File requirements
The Optimizer accepts a **`.csv`** file, **UTF-8** text (with or without UTF-8 BOM), **comma** or **semicolon** as delimiter, a size from **1 KiB to 10 MiB**, no more than **50,000 data rows** and no more than **200 columns**.

Files such as `.xlsx`, UTF-16 files or files with unsupported separators cannot be imported. CSV reports containing no usable data are rejected.

## Required columns
Your report needs all 13 data categories below; AdPilot recognizes several English and Italian header aliases:

| Data | Typical English header | Typical Italian header |
| --- | --- | --- |
| Campaign | Campaign name | Nome della campagna |
| Ad set | Ad set name | Nome del gruppo di inserzioni |
| Audience / interest | Audience/Interest | Pubblico/Interesse |
| Spend | Amount spent | Importo speso |
| Impressions | Impressions | Impression |
| Reach | Reach | Copertura |
| Frequency | Frequency | Frequenza |
| Clicks | Link clicks | Clic sul link |
| Click-through rate | CTR | CTR |
| Cost per click | CPC | CPC |
| Cost per thousand | CPM | CPM |
| Purchases | Purchases | Acquisti |
| Purchase value | Purchase value | Valore conversione acquisti |

Include both **Purchases** and **Purchase value** as distinct fields. If AdPilot reports missing columns, follow [Fix CSV import errors](../troubleshooting/csv-errors.md) and inspect the original headers.

## Prepare reliable data
- Export **one campaign per CSV file**. Avoid combining several campaigns, especially when different campaigns reuse the same ad set name.
- Use plain numeric amounts: for example **1234.56** (comma-delimited CSV) or **1234,56** (semicolon-delimited CSV). Avoid thousands separators such as `1,234.56` or `1.234,56`, which can be interpreted incorrectly.
- Keep descriptions and labels on a single line where possible; line breaks inside quoted CSV cells may not import reliably.
- Use the actual **purchase conversion value**, **not purchase ROAS**, in the purchase-value column. These are different metrics.
- Keep one consistent reporting period and currency, and compare the resulting totals with Meta before acting on AI recommendations.

The **Audience/Interest** field is mandatory for this version of the importer. Meta's standard reports may not offer an equivalent field. **Do not rename an unrelated field or invent targeting values** just to satisfy the importer. If your authentic report lacks the field, ask AdPilot support about a compatible report instead.
