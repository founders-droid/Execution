---
name: critique-product-strategy
description: Provide a critique of a product strategy document
argument-hint: [strategy document]
context: fork
disable-model-invocation: true
user-invocable: true
---

Provide a product strategy critique of the specified product strategy: $ARGUMENTS

Play devil's advocate and point out flaws or limitations in the provided product strategy. Don't be nice! Point out in detail why the product strategy may not work, what questions remain unaddressed, and where the strategy falls short.

## Workflow

1. Verify that the product strategy addresses each of the following 6 strategic questions. If a strategic question is left unaddressed, call it out clearly:

   - Target audience
   - Problem to solve \ Problem you're solving
   - Value proposition
   - Competitive advantage \ strategic differentiation
   - Growth strategy \ channel strategy
   - Business model \ monetization strategy

2. Leverage the following knowledge files to critique each of the dimensions of the product strategy. Read each one (they are in this skill's `best-practices/` folder) before critiquing. Your goal is NOT to rewrite the strategy to be better. Instead it's to provide detailed critiques of what's wrong with the strategy and where it could be stronger.

   @best-practices/what-great-product-strategy-looks-like.md
   @best-practices/target-audience.md
   @best-practices/problem-youre-solving.md
   @best-practices/value-proposition.md
   @best-practices/strategic-differentiation.md
   @best-practices/channel-strategy.md
   @best-practices/monetization-strategy.md

3. Wrap up with a summary of the key critiques you have on the product strategy.

4. Save the entire critique into a markdown file in the same directory as the original product strategy, with the same filename but with '-critique' appended to the end. For example, if the original product strategy is at 'projects/product-x/strategy.md', save your critique to 'projects/product-x/strategy-critique.md'.

   If the strategy was pasted or shared as an image rather than a file, save to `strategy/critiques/YYYY-MM-DD-<kebab-strategy-name>-critique.md`.

## Critique format

```markdown
# Critique: <strategy name>

## Coverage of the 6 strategic questions
| Question | Addressed? (Yes / Partly / No) | Where it falls short |
|---|---|---|
| Target audience | | |
| Problem you're solving | | |
| Value proposition | | |
| Strategic differentiation | | |
| Growth / channel strategy | | |
| Business / monetization model | | |

## Where to play
### Target audience
### Problem you're solving

## How to win
### Value proposition
### Growth / channel strategy
### Business / monetization model

## How to endure
### Strategic differentiation

## Unanswered questions
- 

## Summary of key critiques
1. 
```
