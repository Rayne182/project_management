# Codex Playbook — Markdown Automation

## Claiming Tasks
1. Locate rows where `Status` is `not-started` or `ready`.
2. Assign yourself in the `Assignee` column and set `Status = in-progress`.
3. Commit with `chore(pm): claim <TASK_ID> - <short title>`.

## Updating Tasks
- Add PR and commit URLs once work is pushed.
- Keep table text concise; move long notes to `TASKS/DETAILS/<TASK_ID>.md`.
- Sync documentation across all impacted repositories before completion.

## Completing Tasks
1. Verify documentation, specs, and tests are updated.
2. Set `Status = completed`.
3. Commit with `chore(pm): complete <TASK_ID> - <short title>`.

## Safeguards
- Only edit rows for tasks you own.
- Resolve merge conflicts by keeping the Markdown table structure intact.
