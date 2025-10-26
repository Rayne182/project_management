# SPEC-003 — Frontend Implementation Guide

Provides direction for the `finomi-app-ts` React Native application.

## Environment & Configuration
- Use Expo application config to surface environment variables.
- Manage API endpoints through `.env` files per environment.
- Ensure feature flags and secrets are never committed.

## Development Checklist
1. Adhere to strict TypeScript typing and ESLint rules.
2. Implement hooks and context providers for shared state.
3. Handle errors gracefully with boundaries and user feedback.
4. Add unit tests (Jest) and integration/E2E coverage (Detox) where appropriate.
5. Update documentation and task boards with completed changes and links.
