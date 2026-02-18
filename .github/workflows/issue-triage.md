---
on:
  issues:
    types: [opened, reopened]

permissions:
  contents: read

safe-outputs:
  add-comment:
    max: 1
  add-labels:
  update-issue:

---

# issue-triage

When a new issue is opened, read it and take the following actions:

## Instructions

1. Read the issue title and description carefully
2. Categorize it as one of: bug, feature-request, question, research, or project-idea
3. Add the appropriate label
4. If it is a project-idea, add a comment acknowledging it and summarizing what would be needed to build it
5. If it is a bug, add a comment asking for reproduction steps if not provided
6. If it is a question, provide a helpful response based on the repo contents
