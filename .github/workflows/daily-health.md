---
on:
  schedule: daily

permissions:
  contents: read
  issues: read
  pull-requests: read

safe-outputs:
  create-issue:
    max: 1

---

# daily-health

Run a daily health check on this repository and all repos under AgentSteve80.

## Instructions

1. Check the repository for:
   - Open issues that have been unresolved for more than 7 days
   - Open pull requests that need attention
   - Recent commits and activity summary
   - Any failing workflows or actions
   - Stale branches that could be cleaned up
2. Check for new reports in the reports/ directory
3. Summarize the overall health of the repository
4. Create a single issue titled "Daily Health Report — [today date]" with:
   - Repository health summary
   - Action items that need attention
   - Stats: open issues, open PRs, commits this week
   - Any recommendations for maintenance
5. Keep the report concise and actionable
