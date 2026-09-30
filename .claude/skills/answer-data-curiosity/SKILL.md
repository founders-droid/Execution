---
name: answer-data-curiosity
description: Answer data questions by querying the database
context: fork
disable-model-invocation: true
user-invocable: true
---

Analyze MySQL database data to answer specific data questions the user submits. For each question, construct the appropriate MySQL query, execute it, and return the results in a clear format.

## Workflow
1. Start by analyzing the database you have access to, understanding the tables and columns available. Summarize the database schema in a concise format.
2. Let the user know that you are ready to answer their data questions. Prompt them to ask any question they have about the data.
3. For each question the user asks, construct the appropriate MySQL query to retrieve the relevant data. Then execute the query against the database.
4. Create an HTML report that includes the original question, the MySQL query used, a neatly formatted table of results, and a visualization that graphs the results. Save this report to `./projects/data-curiosity/answer-<timestamp>.html`.
5. Open the HTML report in the user's default web browser to verify successful generation.
