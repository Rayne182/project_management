# Codex Command — Task Handling via Markdown Tables

Source of truth: `/TASKS/PHASE_*` boards.
Each task has a detail file in `/TASKS/DETAILS/<TASK_ID>.md`.

**Process**
1. Find tasks with `status=not-started` or `ready`.
2. Set `status=in-progress`, fill `assignee`.
3. After completion, update PR and commit links, mark as `completed`.
