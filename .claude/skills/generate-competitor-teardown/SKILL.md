---
name: generate-competitor-teardown
description: Produce a competitor teardown — positioning, target users, key features, pricing, strengths, weaknesses, and implications for us — and save it to competitors/teardowns/. Use when the user runs /generate-competitor-teardown or asks for a competitive analysis of a specific company or product.
---

# Generate competitor teardown

## Steps
1. **Collect input.** The competitor's name or URL, plus any notes, screenshots, or docs the user provides.
2. **Research.** If web access is available, use the competitor's site, pricing page, docs, changelog, and reviews (G2, Capterra, app stores).
   - Cite a source for every factual claim.
   - Mark anything not verified as `Unverified`.
   - Never make up numbers.
3. **Tear down** the competitor using the template below. Keep every section short and factual.
4. **Explain what it means for us.** Cover where we win, where we lose, what to copy, what to ignore, and what to watch.
5. **Save** to `competitors/teardowns/<kebab-competitor>.md`. If the file already exists, update it, and add a dated entry to its **Change log**.
6. **Report back** with the 3 most important implications.

## Template
```markdown
# Competitor teardown: <name>
- **Last updated:** YYYY-MM-DD · **Website:** <url>

## Summary
- <who they are + threat level: High | Medium | Low, and why>

## Positioning
- Tagline / core promise:
- Target users & segments:

## Product
| Capability | Them | Us | Notes |
|---|---|---|---|

## Pricing
| Plan | Price | Key limits |
|---|---|---|

## Strengths / Weaknesses
- **Strengths:** 
- **Weaknesses (incl. from reviews):** 

## Implications for us
- Win / Lose / Copy / Ignore / Watch

## Sources
- 

## Change log
- YYYY-MM-DD — created
```
