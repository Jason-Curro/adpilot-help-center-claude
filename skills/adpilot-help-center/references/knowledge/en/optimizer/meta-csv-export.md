---
id: "meta-csv-export"
title: "Export a Meta Ads report"
description: "Prepare a report for the AdPilot Optimizer."
category: "optimizer"
feature: "optimizer"
audience: "merchant"
difficulty: "beginner"
language: "en"
plans: ["PRO"]
keywords: ["meta", "ads manager", "export", "csv", "report"]
last_reviewed: "2026-11-17"
translation_id: "meta-csv-export"
related: ["csv-requirements", "upload-csv"]
---

# Export a Meta Ads report

## Prepare the report in Meta
Meta Ads Manager may change its interface. The following is the workflow described by AdPilot's current in-app instructions:

1. Open **Meta Ads Manager** and go to the reporting area (Reports / Custom report).
2. Choose the reporting date range; AdPilot suggests recent data such as **7–30 days**.
3. Select the campaign you want to analyze and use the **Ad set** level; prepare **one campaign per file**.
4. Include the metrics in [CSV format and required columns](../optimizer/csv-requirements.md), especially **purchase value** (not purchase ROAS).
5. Check whether the reporting layout actually provides **Audience/Interest** or a compatible column. AdPilot requires it, but Meta may not expose that field in its standard report; do not fabricate or mislabel a substitute.
6. Export as **CSV** (not Excel `.xlsx`) and check the downloaded headers and numeric format.
7. Keep the exported file on your device until you upload it to AdPilot.

If Meta offers different report labels, compare the exported CSV headers with [CSV format and required columns](../optimizer/csv-requirements.md). The audience/interest field is mandatory for the current import process. If the authentic Meta export lacks it, request guidance from AdPilot support rather than guessing a substitute.

Do not send private advertising reports to a public chat. See [Upload a CSV to the Optimizer](../optimizer/upload-csv.md).
