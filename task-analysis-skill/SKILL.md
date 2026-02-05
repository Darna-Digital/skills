---
name: task-analysis-skill
description: Analyses a task with the context of the codebase
---

## What I do

1. Ask user for task context
2. Expect to get Slack messages, Jira ticket info, maybe screenshots
3. Understand the intent of the task
4. Analyse this codebase for relevant information
5. Analyse the existing features for how to structure testable code
6. Determine if we should adjust existing feature or create a new feature
7. Finally, create a plan for implementation. Write it in a md file in .opencode/skill/task-analysis-skill/analyses
8. If the branch includes a task slug, (e.g. task/HNV3-1579-fe-missing-order-tracking-id), then prefix the analysis with that task number

## How to use me

Call me in a chat, otherwise I won't load the context.
