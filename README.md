# Zamith Work

### Private AI Operating Layer for Teams and Companies

**Zamith Work** is a long-term AI product concept for securely connecting company knowledge, tools, workflows, and people through one controlled AI layer.

The goal is not to build another generic chatbot. Zamith Work is intended to become a practical company AI system that can understand internal knowledge, use approved tools, assist with multi-step work, and keep sensitive actions under human control.

## Product vision

A company should be able to connect Zamith Work to selected internal systems such as:

- Documents and knowledge bases
- Email and calendar
- CRM and databases
- Internal APIs and business tools
- Team workflows
- Approved external services

Employees can then ask for work in natural language while the system respects role, permission, data scope, and approval boundaries.

## Core principles

- **Private by design** — company data remains controlled and scoped.
- **Permission aware** — users and agents only access what they are allowed to access.
- **Human-approved actions** — sensitive operations require explicit confirmation.
- **Auditable** — important actions and tool usage are traceable.
- **Model independent** — the underlying LLM can be replaced as better models appear.
- **Measurable** — reliability, latency, task success, and regressions are evaluated.
- **Deployable** — designed toward cloud, private-cloud, and on-premise options.

## Planned capabilities

### Company knowledge
- RAG over internal documents
- Source citations
- Permission-aware retrieval
- Freshness and re-indexing
- Project and team knowledge scopes

### Memory
- User memory
- Team/project memory
- Session memory
- Editable and inspectable long-term memory
- Conflict and stale-memory handling

### Tools and integrations
- Email
- Calendar
- Files
- Databases
- CRM
- Search
- Internal APIs
- MCP-compatible services

### Agentic workflows
- Multi-step task execution
- Tool selection
- Retry and fallback
- Human-in-the-loop approvals
- Task status and completion verification

### Security and governance
- Authentication
- Authorization
- Role-based access
- Secret management
- Audit logs
- Data isolation
- Rate limiting
- Safe tool execution

### Evaluation and observability
- Test scenarios
- Regression testing
- RAG evaluation
- Tool-call success metrics
- Agent task-completion metrics
- Latency and failure monitoring

## Example future workflow

```text
Employee request
      ↓
Identity + permissions
      ↓
Retrieve approved company context
      ↓
Plan task
      ↓
Use approved tools
      ↓
Request human approval if needed
      ↓
Execute
      ↓
Verify result
      ↓
Audit + final response
```

Example:

> "Review the latest emails from Client X, find the current contract, summarize the open issues, and prepare a reply for my approval."

Zamith Work should retrieve only authorized information, prepare the work, and stop for approval before performing any sensitive external action.

## Planned architecture

```text
Web / Desktop / Mobile Client
            ↓
        API Gateway
            ↓
 Identity & Permission Layer
            ↓
       AI Orchestrator
      ↙      ↓       ↘
    RAG    Memory    Agents
      ↘      ↓       ↙
        Tool Layer / MCP
             ↓
Documents • Email • Calendar • CRM • Databases • Internal APIs
             ↓
      Audit & Evaluation
```

The architecture is intentionally modular so the LLM, vector store, speech stack, integrations, and deployment model can evolve without rebuilding the entire product.

## Development stages

**Phase 0 — Product definition**  
Define use cases, threat model, success criteria, architecture, and evaluation strategy.

**Phase 1 — Secure knowledge assistant**  
Authentication, permissions, document ingestion, RAG, citations, and evaluation.

**Phase 2 — Business tools**  
Email, calendar, file, database, and internal API integrations.

**Phase 3 — Controlled agent workflows**  
Multi-step execution, human approval, retries, task state, and verification.

**Phase 4 — Company-ready platform**  
Multi-user isolation, audit logs, admin controls, monitoring, backup, and deployment options.

**Phase 5 — Commercial readiness**  
Tenant management, onboarding, billing boundaries, support tooling, documentation, and production hardening.

## What this repository will demonstrate

This project is intended to demonstrate applied AI engineering across:

- AI system architecture
- LLM integration
- RAG
- Memory
- Tool calling
- MCP
- Agents
- API/backend design
- Evaluation and testing
- Performance engineering
- Deployment and security

## Current status

**Planning / architecture stage.**

No production claims are made yet. Features will be marked complete only after implementation and evaluation.

## Relationship to other Zamith projects

- **Zamith Assistant** — personal local-first AI assistant
- **Zamith Work** — company and team AI operating layer
- **Zamith Guardian** — future control, governance, and trust layer for AI agents

Each product is maintained as an independent repository.

## Author

**Amin Bakhtiari**  
AI system builder focused on applied AI products, architecture, evaluation, and product engineering.
