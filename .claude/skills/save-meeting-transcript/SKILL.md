---
name: save-meeting-transcript
description: Save a raw meeting transcript (pasted text or a file) to meetings/transcripts/ with a metadata header, lightly cleaned but not summarized. Use when the user runs /save-meeting-transcript or asks to store or archive a transcript.
---

# Save meeting transcript

Save the transcript as a faithful record. Don't summarize it or rewrite it.

## Steps

1. **Collect input.** Use pasted text, a file path, or text after the command. If nothing was given, ask for the transcript and stop.
2. **Work out the metadata.** Get the title, date, attendees, and length from the input. If the date is missing, use today's date. Don't invent anything. If a value is unknown, write "Not captured".
3. **Clean up lightly.** Only these changes are allowed:
   - Put each speaker turn on its own line, formatted as `**Speaker:** text` (keep timestamps if the input has them).
   - Remove noise lines such as "[inaudible]" repeats, system join/leave messages, and duplicate lines.
   - Don't change any spoken words.
4. **Flag sensitive content.** If the transcript contains passwords, API keys, personal phone numbers, or similar, replace each one with `[REDACTED]` and tell the user what you redacted.
5. **Save** to `meetings/transcripts/YYYY-MM-DD-<kebab-case-title>.md`. If that file already exists, add `-2`, `-3`, and so on.
6. **Report back** with the file path, the number of speaker turns, and any redactions. Then offer to run `/save-meetings` to create structured notes from this transcript.

## File format

```markdown
# Transcript: <Meeting title>

- **Date:** YYYY-MM-DD
- **Attendees:** <names>
- **Duration:** <e.g., 45 min, or "Not captured">
- **Source:** <e.g., Zoom, Google Meet, Otter, pasted>
- **Notes:** <link to meetings/notes/... if it exists>

---

**Speaker A:** ...
**Speaker B:** ...
```
