---
name: save-meetings
description: Turn raw meeting notes, a recap, or a transcript into structured meeting notes (summary, decisions, action items) and save them to meetings/notes/. Use when the user runs /save-meetings or asks to save, log, or record a meeting.
---

# Save meeting notes

Turn whatever the user gives you (pasted notes, bullet points, a transcript, or a file path) into structured notes, then save them.

## Steps

1. **Collect input.** Use the text after the command, pasted content, or a file path. If nothing was given, ask for the notes and stop.
2. **Work out the metadata.** Get the title, date, and attendees from the input. If the date is missing, use today's date. If the title is missing, write a short descriptive one. Don't invent attendees. If they're unknown, write "Not captured".
3. **Write the notes** using the template below. Rules:
   - Use plain language. Define any jargon the first time it appears.
   - Every action item needs an owner and a due date. If either is missing, write `TBD` and list it under Open questions.
   - Record only decisions that were actually made. Anything still being discussed goes under Open questions.
4. **Save** to `meetings/notes/YYYY-MM-DD-<kebab-case-title>.md`. If that file already exists, add `-2`, `-3`, and so on.
5. **Link the transcript.** If a matching transcript exists in `meetings/transcripts/` (same date and a similar title), link it under **Source**.
6. **Report back** with the file path, the 1–3 bullet summary, and the action items table.

## Template

```markdown
# <Meeting title>

- **Date:** YYYY-MM-DD
- **Attendees:** <names>
- **Type:** <e.g., standup, planning, review, 1:1, customer call>
- **Source:** <link to transcript, or "Notes provided by user">

## Summary
- <1–3 bullets: what happened and why it matters>

## Decisions
| # | Decision | Rationale | Owner |
|---|----------|-----------|-------|

## Action items
| # | Action | Owner | Due | Status |
|---|--------|-------|-----|--------|

## Discussion notes
- <key points, grouped by topic>

## Risks / blockers
- <risk — impact — mitigation>

## Open questions
- <question — who can answer>
```
