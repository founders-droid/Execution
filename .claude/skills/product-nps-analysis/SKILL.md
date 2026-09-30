---
name: product-nps-analysis
description: Analyze Net Promoter Score (NPS) survey results — score, trend, segment breakdown, and themes from verbatim comments — and save actionable findings to research/nps/. Use when the user runs /product-nps-analysis or shares NPS or survey data.
---

# Product NPS analysis

NPS (Net Promoter Score) = % Promoters (9–10) − % Detractors (0–6). Passives (7–8) count in the total but not in either group.

## Steps
1. **Collect input.** A CSV or pasted responses with the score, and ideally a comment, date, and segment (plan, role, tenure). Note any columns that are missing.
2. **Calculate.**
   - Overall NPS, the number of responses, and the margin of error. Flag the result as low-confidence if there are fewer than 100 responses.
   - Break down by segment and by period, if dates exist.
3. **Code the themes.** Tag each comment with 1–2 themes. Count the themes separately for Promoters, Passives, and Detractors.
4. **Find the levers.** Name the top 3 Detractor themes (what to fix) and the top 3 Promoter themes (what to protect and market). Quote 1–2 real comments for each. Don't invent quotes.
5. **Recommend** actions with impact and effort (S/M/L) and the metric to watch.
6. **Save** to `research/nps/YYYY-MM-DD-nps.md`. Report the score, trend, and top actions.

## Template
```markdown
# NPS analysis — <period>

## Summary
- NPS **<score>** (n=<N>, ±<moe>) — <trend vs. last period>
- <top insight>

## Breakdown
| Segment | n | Promoters | Passives | Detractors | NPS |
|---|---|---|---|---|---|

## Themes
| Theme | Detractors | Passives | Promoters | Example quote |
|---|---|---|---|---|

## Recommended actions
| Action | Theme addressed | Impact | Effort | Metric |
|---|---|---|---|---|

## Data caveats
- 
```
