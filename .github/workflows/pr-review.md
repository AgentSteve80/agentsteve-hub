---
on:
  pull_request:
    types: [opened, synchronize]

permissions:
  contents: read
  pull-requests: read

safe-outputs:
  add-comment:
    max: 1
  add-labels:

---

# pr-review

When a pull request is opened or updated, review the changes and provide feedback.

## Instructions

1. Read the PR title, description, and all changed files
2. Review the code for:
   - Bugs or logic errors
   - Security vulnerabilities (injection, hardcoded secrets, unsafe inputs)
   - Code quality and readability
   - Missing tests for new functionality
   - Breaking changes
3. Add a label: needs-review, approved, or changes-requested
4. Add a single comment summarizing your review with:
   - What the PR does (1-2 sentences)
   - Any issues found (with file and line references)
   - Suggestions for improvement
   - Overall assessment: approve, request changes, or needs discussion
5. Be constructive and specific — no vague feedback
