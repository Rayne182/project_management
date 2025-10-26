# Finomi Coding Standards

## Frontend (`finomi-app-ts`)
- Language: TypeScript (strict mode)
- Framework: Expo + React Native
- Linting: ESLint + Prettier (CI enforced)
- Testing: Jest for unit, Detox for E2E
- Configuration: Use environment files and `app.config.ts`

## Backend (`Finomi.App.Api`)
- Language: C# (.NET 8)
- ORM: Entity Framework Core
- Testing: xUnit unit/integration coverage for services and controllers
- Security: JWT authentication with role-based authorization

## Documentation & Tracking (`project_management`)
- All work items live in Markdown tables under `TASKS/`
- Keep task detail pages synchronized with spec references and links
- Reference supporting specs for implementation guidance

## Commit Messages
Use [Conventional Commits](https://www.conventionalcommits.org/) across all repositories.
