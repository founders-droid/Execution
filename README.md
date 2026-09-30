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
| `/analyze-pricing-change` | Models revenue and churn impact of a pricing change, with break-even and a recommendation | `pricing/` |
| `/answer-data-curiosity` | Answers an ad-hoc data question with evidence and a confidence level | `data-questions/` |
| `/product-nps-analysis` | Calculates NPS, breaks it down by segment, and codes comment themes into actions | `research/nps/` |
| `/critique-product-strategy` | Scores a strategy across 7 areas and lists top weaknesses, fixes and risky assumptions | `strategy/critiques/` |
| `/generate-competitor-teardown` | Builds a sourced teardown of one competitor and what it means for us | `competitors/teardowns/` |
| `/generate-interview-script` | Writes a non-leading, time-boxed customer interview script | `research/interview-scripts/` |
| `/generate-weekly-dashboards` | Builds a weekly metrics report with week-over-week change, status and actions | `dashboards/` |
| `/summarize-customer-interviews` | Synthesizes interviews into counted themes, quotes and jobs-to-be-done | `research/interviews/` |
| `/update-competitor-pricing` | Refreshes the competitor pricing tracker and logs changes | `competitors/pricing.md` |

The command definitions live in `.claude/skills/<command>/SKILL.md`.

## Folder layout
```
meetings/
  notes/         structured meeting notes
  transcripts/   raw transcripts
  agendas/       meeting agendas
release-notes/   one file per release
pricing/         pricing change analyses
data-questions/  answered data questions
research/        nps/, interviews/, interview-scripts/
strategy/        critiques/
competitors/     teardowns/ and pricing.md
dashboards/      weekly dashboards (YYYY-Www.md)
```

Files are named `YYYY-MM-DD-<title>.md` so they sort by date.
