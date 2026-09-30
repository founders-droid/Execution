---
name: summarize-customer-interviews
description: Synthesize one or more customer interview transcripts or notes into themes, pain points, quotes, jobs-to-be-done, and product implications, and save to research/interviews/. Use when the user runs /summarize-customer-interviews or asks to synthesize user research.
---

# Summarize customer interviews

JTBD (jobs-to-be-done) is the underlying goal a customer is trying to get done: "When <situation>, I want to <motivation>, so I can <outcome>."

## Steps
1. **Collect input.** Transcripts or notes, pasted or as files. Use `meetings/transcripts/` or `research/` if the user points there.
2. **Summarize each interview.** Write 3–5 bullets per interview, covering the participant's profile (role, segment), top pains, current workaround, and notable quotes.
3. **Synthesize across interviews.**
   - Group the findings into themes and count how many participants mentioned each theme (e.g., 4/6).
   - A theme mentioned by only 1 person is a *signal*, not a theme.
   - Write the JTBD statements.
4. **Quote exactly.** Use verbatim quotes only, attributed as "P1, P2…". Never change or invent quotes. Remove names unless the user says otherwise.
5. **Draw implications.** For each top theme, give the opportunity, the confidence level, and the next step: build, test, or research more.
6. **Save** to `research/interviews/YYYY-MM-DD-<kebab-topic>.md`. Report the top 3 themes with their counts.

## Template
```markdown
# Interview synthesis: <topic>
- **Date:** YYYY-MM-DD · **Participants:** <N> (<segments>)

## Summary
- <top 1–3 insights>

## Themes
| Theme | Mentions | Representative quote | Implication |
|---|---|---|---|

## Jobs to be done
- When …, I want to …, so I can …

## Signals (single mentions worth watching)
- 

## Per-participant notes
### P1 — <role, segment>
- 

## Next steps
| Opportunity | Confidence | Next step | Owner |
|---|---|---|---|
```
