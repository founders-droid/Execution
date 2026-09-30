---
name: update-competitor-pricing
description: Refresh the competitor pricing tracker — current plans, prices, and limits per competitor, with dated changes — in competitors/pricing.md. Use when the user runs /update-competitor-pricing or asks to check or log competitor price changes.
---

# Update competitor pricing

## Steps
1. **Load the tracker.** Open `competitors/pricing.md`. If it doesn't exist, create it from the template below.
2. **Choose which competitors to update.** Use the ones the user names. If none are named, update every competitor already in the tracker.
3. **Get current pricing.**
   - If web access is available, use each competitor's pricing page.
   - Otherwise, use what the user provides.
   - Record the source URL and the date checked.
   - Never guess a price. If you can't verify a price, keep the old value and mark it `Unverified as of YYYY-MM-DD`.
4. **Compare** against the tracker. For every change (price, plan name, limits, new or removed plan), add a row to the **Change log**.
5. **Flag what matters to us.** Point out any change that affects our position, such as a competitor now undercutting us on a key plan. Suggest running `/analyze-pricing-change` when a response may be needed.
6. **Save** the tracker. Report what changed; if nothing changed, say "No changes".

## Template (competitors/pricing.md)
```markdown
# Competitor pricing tracker
- **Last updated:** YYYY-MM-DD

## Current pricing
| Competitor | Plan | Price (monthly / annual) | Key limits | Source | Checked |
|---|---|---|---|---|---|

## Change log
| Date | Competitor | Change | Before | After | Implication for us |
|---|---|---|---|---|---|
```
