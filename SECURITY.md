# Security Principles

Zamith Work is intended to handle company information and potentially execute business actions. Security is therefore a product requirement, not a later add-on.

## Core rules

1. **Least privilege** — users, services, and agents receive only the minimum access required.
2. **Explicit approval** — sensitive or external actions require human confirmation unless a narrowly defined policy explicitly allows them.
3. **Data isolation** — one user, team, project, or tenant must not retrieve data outside its permitted scope.
4. **No secrets in source code** — credentials belong in approved secret stores or environment configuration.
5. **Untrusted content stays untrusted** — retrieved documents, web pages, emails, and tool output must not silently override system policy.
6. **Auditable actions** — privileged operations must be traceable.
7. **Safe failure** — when identity, permission, or policy is uncertain, the system should not perform the action.
8. **Reversible operations where possible** — destructive actions require stronger confirmation.
9. **Separation of model and authority** — an LLM may recommend an action; the application decides whether it is permitted.
10. **Evaluation before release** — security-sensitive behavior must have regression tests.

## Planned security areas

- Authentication
- Authorization
- Role-based access control
- Tenant isolation
- Tool permissions
- Human approval
- Input validation
- Prompt-injection resistance
- Secret management
- Encryption
- Logging and audit
- Rate limiting
- Backup and recovery
- Dependency security
- Deployment hardening

## Disclosure

This repository is currently in planning/development stage and should not be treated as production-ready security software.
