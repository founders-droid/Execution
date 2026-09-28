# Execution
All things product execution related including meetings

## Commands
Run these in Claude Code with this repository open.

| Command | What it does | Saves to |
|---------|--------------|----------|
| `/save-meetings` | Turns raw notes or a transcript into structured notes: summary, decisions, action items | `meetings/notes/` |
| `/save-meeting-transcript` | Stores a raw transcript with a metadata header (cleaned up, not summarized) | `meetings/transcripts/` |
| `/draft-meeting-agenda` | Drafts a time-boxed agenda and carries forward open items from the last meeting | `meetings/agendas/` |
| `/generate-release-notes` | Writes plain-language release notes from changes, PRs, or commits | `release-notes/` |

The command definitions live in `.claude/skills/<command>/SKILL.md`.

## Folder layout
```
meetings/
  notes/         structured meeting notes
  transcripts/   raw transcripts
  agendas/       meeting agendas
release-notes/   one file per release
```

Files are named `YYYY-MM-DD-<title>.md` so they sort by date.
