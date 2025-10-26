# QA Testing Guide

1. Review the relevant task detail page for acceptance criteria.
2. Execute automated test suites (frontend Jest/Detox, backend xUnit/integration) when applicable.
3. Perform manual smoke tests covering:
   - Authentication flows
   - Core data interactions
   - Error handling and boundary conditions
4. Document findings in `REPORTS/QA_REPORT_TEMPLATE.md` or phase-specific QA logs.
5. Block tasks with discovered defects and note remediation steps in the task detail page.
