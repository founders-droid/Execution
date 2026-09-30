---
name: answer-data-curiosity
description: Answer an ad-hoc data question ("why did X drop?", "how many users do Y?") by framing it, finding or requesting the data, analyzing it, and writing a short answer with confidence level to data-questions/. Use when the user runs /answer-data-curiosity or asks a quick product-data question.
---

# Answer data curiosity

## Steps
1. **Restate the question** as something that can be measured: metric, segment, time range, and comparison. If it's vague, pick the most likely reading and say so.
2. **Find the data.** Use files, CSVs, or query results the user provided, or data in the repo.
   - If there's no data, write the query or the exact data pull needed (e.g., SQL with table and column placeholders), then stop and ask the user to run it.
3. **Analyze.**
   - Start with the headline number, then break it down by the likely drivers: segment, platform, time, cohort (a group of users who started in the same period).
   - Check for data problems first: tracking changes, outages, seasonality.
4. **Answer plainly.** Give one sentence of answer, the supporting numbers, and a confidence level (High, Medium, or Low) with the reason for it.
5. **Suggest a follow-up.** Name what would raise confidence, or the next question worth asking.
6. **Save** to `data-questions/YYYY-MM-DD-<kebab-question>.md`. Report the answer and confidence.

## Template
```markdown
# Q: <question>
- **Date:** YYYY-MM-DD · **Asked by:** <name or "Not captured">

## Answer
<one sentence> — **Confidence:** High | Medium | Low (<why>)

## Evidence
| Cut | Value | Change |
|---|---|---|

## Method
- Data source, filters, time range
- Query (if any)

## Caveats
- 

## Follow-ups
- 
```
