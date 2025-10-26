# Agent Operations Guide

This repository is the control center for Finomi delivery. Follow these rules while working anywhere under `project_management/`.

## Workflow Summary
1. Work exclusively from Markdown task boards under `TASKS/`.
2. Claim tasks before beginning work, update status and assignee in the board.
3. Maintain links to task details, PRs, and commits inside each table row.
4. Update related Finomi repositories (`finomi-app-ts`, `Finomi.App.Api`, and `project_management`) before marking tasks complete.
5. Keep Markdown tables tidy—do not break formatting or reorder columns.

## Status Flow
`not-started → in-progress → completed` with optional `ready` and `blocked` states when applicable.

## Commit Conventions
Use Conventional Commits:
- `chore(pm): claim TASK_ID - <short title>` when starting a task.
- `chore(pm): complete TASK_ID - <short title>` when finishing.
- Use other prefixes (`feat`, `fix`, `docs`) as appropriate for supporting repositories.

See supporting guides within this folder for coding standards, QA practices, PR templates, and compliance requirements.
