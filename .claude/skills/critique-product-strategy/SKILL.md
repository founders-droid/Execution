---
name: critique-product-strategy
description: Critique a product strategy, roadmap, or plan — test it for clarity, evidence, differentiation, feasibility, and measurable outcomes — and save a scored critique with concrete fixes to strategy/critiques/. Use when the user runs /critique-product-strategy or asks for feedback on a strategy doc.
---

# Critique product strategy

Be direct and specific. Critique the strategy, not the writing style.

## Steps
1. **Collect input.** A doc, file, link, or pasted text. Before critiquing, restate the strategy in 3 bullets: who it's for, what problem it solves, and the bet being made.
2. **Score each area from 1 to 5**, with a one-line reason:
   - **Target user & problem:** Is it specific? Is there evidence the problem is real and painful?
   - **Desired outcome & metrics:** Is there a North Star metric (the one number that shows success) plus input metrics? Are there targets and dates?
   - **Differentiation:** Why do we win? Why can't competitors copy it quickly?
   - **Choices & non-goals:** Does it say what we will *not* do?
   - **Feasibility:** Are resources, dependencies, and sequencing realistic?
   - **Risks:** Are the biggest assumptions named? Is there a plan to test them?
   - **Go-to-market & monetization:** How does the product reach users, and how does it make money?
3. **List the top 3 weaknesses**, most serious first. For each, give a concrete fix and a question to ask the author.
4. **List the riskiest assumptions** and the cheapest way to test each one.
5. **Give a verdict:** Ready, Ready with fixes, or Rework.
6. **Save** to `strategy/critiques/YYYY-MM-DD-<kebab-name>.md`. Report the verdict and top 3 fixes.

## Template
```markdown
# Strategy critique: <name>
- **Date:** YYYY-MM-DD · **Verdict:** Ready | Ready with fixes | Rework

## The strategy in 3 bullets
- 

## Scorecard
| Area | Score (1–5) | Why |
|---|---|---|

## Top weaknesses & fixes
1. **<weakness>** — Fix: … — Ask: …

## Riskiest assumptions
| Assumption | Why risky | Cheapest test |
|---|---|---|

## What's strong
- 
```
