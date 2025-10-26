# Finomi Project Management Repository

The **Finomi Project Management** repository is the single source of truth for tracking and delivering Finomi product work. It replaces spreadsheets and external tools with Markdown-based workflows that Codex agents and engineers can edit collaboratively.

## Purpose
- Provide a transparent, automation-friendly backlog for Codex agents, PMs, and engineers.
- Keep cross-repository documentation synchronized across `finomi-app-ts`, `Finomi.App.Api`, and `project_management`.
- Maintain centralized specifications, reports, and automation playbooks for the Finomi program.

## Repository Layout
```
project_management/
├── README.md
├── AGENTS/
│   ├── AGENTS.md
│   ├── CODING_STANDARDS.md
│   ├── PR_TEMPLATE.md
│   ├── QA_TESTING_GUIDE.md
│   └── SECURITY_AND_COMPLIANCE.md
├── SPECS/
│   ├── SPEC-001_TASK_DETAILING_FOR_JUNIOR_ENGINEERS.md
│   ├── SPEC-002_BACKEND_IMPLEMENTATION_GUIDE.md
│   ├── SPEC-003_FRONTEND_IMPLEMENTATION_GUIDE.md
│   └── SPEC-004_POPIA_AND_FSCA_COMPLIANCE_BASELINE.md
├── TASKS/
│   ├── INDEX.md
│   ├── ROADMAP.md
│   ├── PHASE_1_FOUNDATION.md
│   ├── PHASE_2_CORE.md
│   ├── PHASE_3_QUALITY.md
│   ├── PHASE_4_ENHANCED.md
│   ├── PHASE_5_LAUNCH.md
│   └── DETAILS/
│       └── FND-001.md
├── REPORTS/
│   ├── WEEKLY_SUMMARY_TEMPLATE.md
│   ├── QA_REPORT_TEMPLATE.md
│   ├── SECURITY_AUDIT_TEMPLATE.md
│   └── PERFORMANCE_METRICS.md
└── AUTOMATION/
    ├── codex_playbook.md
    ├── notion_sync_job.yaml
    └── github_actions_pipeline.yaml
```

## Core Workflow
1. **Track Tasks** – Each phase board uses Markdown tables with consistent columns (`TASK_ID`, `Status`, etc.).
2. **Update Status Flow** – `not-started → in-progress → completed` with optional `ready` and `blocked` states.
3. **Automate with Codex** – Agents claim tasks, implement work, and update PR + commit references directly in the tables.
4. **Cross-Repo Compliance** – Completed work must update documentation in all related Finomi repositories.

See [`AGENTS/AGENTS.md`](AGENTS/AGENTS.md) for day-to-day operating guidance.
