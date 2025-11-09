# QA Manual Test Plan â€” Phase 1 & 2 (Ready-To-Test)

Test Execution Tracker (Index)

| Task ID | Title | Detail | Status | Comments |
|---|---|---|---|---|
| [FND-001](./QA_PLANS/FND-001.md) | Environment-Based API Configuration | [Task Detail](../TASKS/DETAILS/FND-001.md) | Passed | Tested with env.development and base URL: http://192.168.80.97:5185/api/v1/ and Create/Login endpoints in UserController using [AllowAnonymous] decorator |
| [FND-002](./QA_PLANS/FND-002.md) | Authentication Token Integration | [Task Detail](../TASKS/DETAILS/FND-002.md) | - | |
| [FND-003](./QA_PLANS/FND-003.md) | Authentication Context Provider | [Task Detail](../TASKS/DETAILS/FND-003.md) | - | |
| [FND-004](./QA_PLANS/FND-004.md) | Remove Hard-Coded User Data | [Task Detail](../TASKS/DETAILS/FND-004.md) | - | |
| [FND-005](./QA_PLANS/FND-005.md) | Implement Error Boundary | [Task Detail](../TASKS/DETAILS/FND-005.md) | - | |
| [FND-006](./QA_PLANS/FND-006.md) | Enforce Authorization and Token Validation | [Task Detail](../TASKS/DETAILS/FND-006.md) | - | |
| [COR-001](./QA_PLANS/COR-001.md) | Implement Transaction Endpoints | [Task Detail](../TASKS/DETAILS/COR-001.md) | - | |
| [COR-002](./QA_PLANS/COR-002.md) | Deposit and Withdrawal Flow | [Task Detail](../TASKS/DETAILS/COR-002.md) | - | |
| [COR-003](./QA_PLANS/COR-003.md) | Activity Screen | [Task Detail](../TASKS/DETAILS/COR-003.md) | - | |
| [COR-004](./QA_PLANS/COR-004.md) | Notifications System | [Task Detail](../TASKS/DETAILS/COR-004.md) | - | |
| [COR-005](./QA_PLANS/COR-005.md) | Settings and Preferences | [Task Detail](../TASKS/DETAILS/COR-005.md) | - | |
| [COR-006](./QA_PLANS/COR-006.md) | State Management and Caching | [Task Detail](../TASKS/DETAILS/COR-006.md) | - | |

Legend

- Status values: not-tested, in-test, passed, failed, rejected, blocked, needs-fix

How To Use

- Click a Task ID to open its dedicated test plan.
- Update Status and Comments in each per-task file as you test.
- Keep this index table in sync with pass/fail outcomes for a quick snapshot.

## Pre-requisites

- Backend running and reachable from device:
   - URL: `http://<LAN_IP>:5185/api/v1/`
   - For dev: disable HTTPS redirect or run HTTP (`--urls http://0.0.0.0:5185`).
   - Windows Firewall allows inbound 5185.
   - Firebase Admin credentials available to API (e.g., `firebase-config.json` at content root or `GOOGLE_APPLICATION_CREDENTIALS` set).

- Frontend env points to LAN IP:
   - `finomi-app-ts/.env.development`: `EXPO_PUBLIC_API_BASE_URL=http://<LAN_IP>:5185/api/v1/`
   - Restart Expo with cache clear: `npx expo start -c`

- Test data: Ensure at least one valid `PaymentMethod` for the test user (or create via DB/endpoint when available).

## Troubleshooting

- 401/403 on signup/login: ensure `[AllowAnonymous]` on `UserController` create/login, FE sends requests to LAN IP.
- 500 on create profile: verify Firebase Admin credentials path is correct and accessible by API.
- Device canâ€™t reach API: confirm LAN IP/port, firewall, and Kestrel binding.

## Reporting

- Use `REPORTS/QA_REPORT_TEMPLATE.md` to log results per task.
- Include:
   - App build/branch, API build/branch
   - Device type, OS version
   - Steps, actual vs expected, logs (client/server), screenshots if helpful


