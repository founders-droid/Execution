---
name: analyze-pricing-change
description: Analyze a proposed or completed pricing change (new price, tier, packaging, discount) for revenue, conversion, churn, and customer impact, and save a decision-ready analysis to pricing/. Use when the user runs /analyze-pricing-change or asks whether to change pricing or how a pricing change performed.
---

# Analyze pricing change

## Steps
1. **Collect input.** Get the change (current vs. proposed), the affected segments, and any data provided (price, customer counts, conversion, churn, ARPU = average revenue per user). If data is missing, use clearly labeled assumptions. Don't stall.
2. **Classify the change.** Is it proposed (forecast) or already launched (measure actual vs. expected)?
3. **Model the impact.** Build three scenarios: Conservative, Base, and Optimistic.
   - Revenue = customers × conversion × price × (1 − churn)
   - Show the break-even: the drop in conversion or rise in churn at which the change stops paying off.
4. **Check customer impact.** Work out who pays more, who pays less, and who is grandfathered (kept on the old price). Name the segments most likely to churn or complain.
5. **Compare competitors.** If `competitors/pricing.md` exists, compare against it.
6. **Recommend** one of: Do it, Test first, or Don't. Include a rollout plan and guardrail metrics.
7. **Save** to `pricing/YYYY-MM-DD-<kebab-change-name>.md`. Report the recommendation and the break-even.

## Template
```markdown
# Pricing change: <name>
- **Date:** YYYY-MM-DD · **Status:** Proposed | Launched

## Summary
- <recommendation + why, 1–3 bullets>

## Change
| | Current | Proposed |
|---|---|---|

## Impact model
| Scenario | Conversion | Churn | Price | Monthly revenue | Δ vs. today |
|---|---|---|---|---|---|

**Break-even:** <e.g., conversion can drop up to X% before revenue falls>

## Customer impact by segment
| Segment | Effect | Risk | Mitigation |
|---|---|---|---|

## Recommendation & rollout
- Test design / rollout steps
- Guardrail metrics: <metric — threshold that triggers rollback>

## Assumptions
- 
```
