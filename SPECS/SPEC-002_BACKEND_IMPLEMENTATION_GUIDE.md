# SPEC-002 — Backend Implementation Guide

Defines patterns and expectations for work in `Finomi.App.Api`.

## Architecture Principles
- Domain-driven structure with clear separation of controllers, services, and data access.
- Use Entity Framework Core for persistence; migrations must be idempotent and source-controlled.
- Apply DTO validation and mapping layers to maintain schema consistency.

## Development Checklist
1. Document new endpoints with request/response schemas.
2. Provide unit and integration tests for API features.
3. Ensure logging, telemetry, and error handling follow observability standards.
4. Enforce security: JWT authentication, role-based authorization, and input validation.
5. Update task boards and detail pages upon completion.
