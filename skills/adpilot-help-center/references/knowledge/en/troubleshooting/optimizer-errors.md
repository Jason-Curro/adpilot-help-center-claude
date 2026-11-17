---
id: "optimizer-errors"
title: "Fix Optimizer access and report issues"
description: "Check plan eligibility, campaigns, waiting time and reports."
category: "troubleshooting"
feature: "troubleshooting"
audience: "merchant"
difficulty: "beginner"
language: "en"
plans: ["PRO"]
keywords: ["optimizer", "error", "locked", "csv", "cooldown"]
last_reviewed: "2026-11-17"
translation_id: "optimizer-errors"
related: ["csv-requirements", "optimization-cooldown", "csv-errors", "error-reference"]
---

# Fix Optimizer access and report issues

## If optimization is unavailable
1. Confirm that your active plan is **Pro**; Free and Starter cannot create new optimization rounds.
2. Open **Campaigns** and select a saved AI proposal. Optimization starts from a saved campaign, not from an arbitrary report on its own.
3. Check whether a **72-hour waiting period** is shown for that campaign.
4. Verify your CSV against [CSV format and required columns](../optimizer/csv-requirements.md).
5. If processing fails with a reference code, record it and the approximate time.

## If recommendations look wrong
Compare spend, purchases, purchase value, date range and campaign/ad-set grouping with the original Meta Ads report. Do not automatically apply an AI suggestion that conflicts with your real performance or advertising rules.

See [When can I optimize again?](../optimizer/optimization-cooldown.md), [Fix CSV import errors](../troubleshooting/csv-errors.md) and [What does ERR-XXXXXX mean?](../troubleshooting/error-reference.md).
