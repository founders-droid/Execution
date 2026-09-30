---
name: generate-interview-script
description: Write a customer interview script (discovery, usability, churn, or win/loss) with goals, screener, warm-up, open-ended non-leading questions, and wrap-up, and save it to research/interview-scripts/. Use when the user runs /generate-interview-script or asks for interview questions.
---

# Generate interview script

## Steps
1. **Collect input.** Get the research goal, the target participant, the interview type (Discovery, Usability, Churn, or Win/Loss), and the length. The default length is 30 minutes.
2. **Set learning goals.** Write 2–4 specific things we need to learn. Every question must map to a goal.
3. **Write the questions.** Rules:
   - Open-ended ("Tell me about the last time…"), not yes/no.
   - Ask about past behavior, not hypotheticals ("Would you use…?" is banned).
   - No leading questions. Don't mention our solution until the final section, if at all.
   - Add 1–2 follow-up probes under each main question ("Why was that?", "What happened next?").
4. **Time-box the sections** so the times add up to the interview length.
5. **Write a screener:** 3–5 questions to confirm a participant fits the target.
6. **Save** to `research/interview-scripts/YYYY-MM-DD-<kebab-topic>.md`. Report the learning goals and the question count.

## Template
```markdown
# Interview script: <topic>
- **Type:** <type> · **Length:** <N> min · **Target participant:** <description>

## Learning goals
1. 

## Screener
- 

## Script
### Intro (2 min)
- Thanks, purpose, no right/wrong answers, permission to record

### Warm-up (3 min)
- Tell me about your role and a typical week.

### Core (N min)
**Goal 1:** …
- Q: Tell me about the last time you… 
  - Probe: …

### Wrap-up (3 min)
- Anything we didn't ask that we should have?
- Who else should we talk to?

## Note-taking grid
| Goal | Key quotes | Observations |
|---|---|---|
```
