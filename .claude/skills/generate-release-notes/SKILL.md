---
name: generate-release-notes
description: Generate plain-language release notes from a list of changes, merged PRs, or git commits, grouped by user impact, and save them to release-notes/. Use when the user runs /generate-release-notes or asks for release notes, a changelog, or a "what shipped" summary.
---

# Generate release notes

Write for customers and stakeholders, not engineers. Lead with what changed for the user and why it matters.

## Steps

1. **Collect input.** Use the first of these that's available:
   1. Changes pasted or listed after the command.
   2. A repo plus a range, e.g. `owner/repo v1.2.0..v1.3.0` or "PRs merged since <date>". Read the merged PRs or commits.
   3. If there's nothing, ask what's in the release and stop.
2. **Get the version and date.** If no version is given, use `YYYY-MM-DD` as the release label.
3. **Sort each change into one of these groups:**
   - **New:** new features or capabilities
   - **Improved:** existing features made better or faster
   - **Fixed:** bug fixes
   - **Changed / Deprecated:** behavior changes users must know about
   - **Internal:** refactors, CI, dependencies, tests. List these only in the Internal section. Leave them out of the Highlights.
4. **Rewrite each change.**
   - One line per change, written from the user's point of view: "You can now…", "Fixed an issue where…".
   - No commit hashes, ticket jargon, or code names in the user-facing sections. Put the PR or issue link at the end of the line.
   - If a change's user impact is unclear, list it under **Needs review** instead of guessing.
5. **Call out breaking changes.** Anything that needs user action goes under **Action required**, at the top, with the exact steps to take.
6. **Save** to `release-notes/<version-or-date>.md`.
7. **Report back** with the file path, the Highlights, and the **Needs review** items.

## Template

```markdown
# Release <version> — YYYY-MM-DD

## Highlights
- <top 1–3 changes and why they matter>

## Action required
- <breaking change — what to do>

## New
- 

## Improved
- 

## Fixed
- 

## Changed / Deprecated
- 

## Internal
- 

## Needs review
- <items with unclear user impact>
```

Leave out any section that has no items, except **Highlights**, which is always included.
