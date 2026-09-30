---
name: generate-weekly-dashboards
description: Build a weekly product metrics dashboard — North Star and input metrics with week-over-week change, highlights, lowlights, and actions — and save it to dashboards/. Use when the user runs /generate-weekly-dashboards or asks for a weekly metrics update or KPI report.
---

# Generate weekly dashboard

## Steps
1. **Collect input.** Get the metric data for this week and last week (CSV, pasted table, or query results).
   - If `dashboards/metrics.md` exists, use it as the list of metrics to track: name, definition, target, and owner.
   - If it doesn't exist, create it from the metrics provided and ask the user to confirm the list.
2. **Calculate** the week-over-week (WoW) change and progress against target for every metric. Give each metric a status:
   - On track: at or above target
   - Watch: within 10% of target
   - Off track
3. **Explain what changed.** For every metric that moved more than 10% WoW or is Off track, give the likely cause.
   - Ground the cause in data or notes the user provided. If none are available, write "cause unknown — investigate".
4. **Write the narrative:** 3 highlights, 3 lowlights, and the actions, each with an owner.
5. **Save** to `dashboards/YYYY-Www.md`, using the ISO week number (e.g., `2026-W40.md`).
6. **Report back** with the summary and the list of Off track metrics.

## Template
```markdown
# Weekly dashboard — <YYYY-Www> (<date range>)

## Summary
- <1–3 bullets: overall health + biggest change>

## North Star
| Metric | This week | Last week | WoW | Target | Status |
|---|---|---|---|---|---|

## Input metrics
| Metric | This week | Last week | WoW | Target | Status | Owner |
|---|---|---|---|---|---|---|

## Highlights
- 

## Lowlights
- 

## Actions
| Action | Owner | Due |
|---|---|---|

## Data notes
- <tracking changes, missing data>
```
