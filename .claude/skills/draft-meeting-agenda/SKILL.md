---
name: draft-meeting-agenda
description: Draft a time-boxed meeting agenda with a clear goal, topics, owners, and pre-reads, and save it to meetings/agendas/. Use when the user runs /draft-meeting-agenda or asks to prepare or plan a meeting agenda.
---

# Draft meeting agenda

## Steps

1. **Collect input.** From the text after the command, get the meeting purpose, date, length, attendees, and topics. Anything missing, fill with a sensible default and list it under **Assumptions**. Don't stop to ask. Defaults:
   - Length: 30 minutes
   - Date: the next business day
2. **Pull in context.** Check `meetings/notes/` for earlier meetings with a similar title or the same attendees.
   - Carry forward any open action items and open questions from the most recent one, under **Follow-ups from last meeting**.
3. **Set one goal.** State the outcome the meeting must produce, e.g., "Decide X" or "Align on Y". If the meeting has no decision or output, suggest handling it asynchronously instead.
4. **Build the agenda.**
   - Time-box every item, and make sure the times add up to the meeting length.
   - Mark each item as Decide, Discuss, or Inform.
   - Put Decide items first.
   - Keep the last 5 minutes for recapping decisions and action items.
5. **Save** to `meetings/agendas/YYYY-MM-DD-<kebab-case-title>.md`. If that file already exists, add `-2`, `-3`, and so on.
6. **Report back** with the file path and the agenda table. Also include a short invite blurb the user can paste into a calendar invite.

## Template

```markdown
# Agenda: <Meeting title>

- **Date / time:** YYYY-MM-DD, <time + timezone>
- **Length:** <N> min
- **Attendees:** <names> (**Facilitator:** <name>, **Note-taker:** <name>)
- **Goal:** <the one outcome this meeting must produce>

## Pre-reads
- <doc/link — why to read it>

## Follow-ups from last meeting
- <open action item — owner — status>

## Agenda
| Time | Topic | Type (Decide/Discuss/Inform) | Owner | Desired outcome |
|------|-------|------------------------------|-------|-----------------|
| 0:00–0:05 | ... | ... | ... | ... |
| ... | Recap decisions + action items | — | Facilitator | Owners and dates confirmed |

## Parking lot
- 

## Assumptions
- <anything defaulted>
```
