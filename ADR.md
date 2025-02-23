# Document Initial ADRs (Architectural Decision Records)
## What is it?

**Architectural Decision Records (ADRs)** is a document that captures key architecture-related decisions, the context in which they were made, and the consequences of the decision. ADRs help teams maintain a historical record of choices, making it easier to understand past decisions and their rationale.

## ADR Tools

- [adr-tools](https://github.com/npryce/adr-tools)

## How to Document ADRs?
Each ADR should follow a standard structure:
1. **Title** – Concise name of the decision.
2. **Status** – Proposed, Accepted, Deprecated.
3. **Context** – Background of the issue being addressed.
4. **Decision** – What choice was made and why.
5. **Consequences** – Trade-offs, risks, and alternative considerations.


## ADR Structure

Each ADR should follow a consistent format for clarity and reusability:

```md
# ADR-XXX: <Decision Title>

## Status
Proposed | Accepted | Deprecated | Superseded

## Context
- What problem are we solving?
- What are the constraints, business needs, and technical considerations?
- What alternatives were considered?

## Decision
- What choice was made and why?
- What trade-offs were considered?
- Why was this chosen over alternatives?

## Consequences
- **Positive Effects** – What benefits does this bring?
- **Negative Effects** – What are the trade-offs or risks?
- **Future Considerations** – When should this decision be re-evaluated?

## References
- Link to discussions, documentation, or external references.

```

## Examples of ADRs

### Example 1: Choosing PostgreSQL as the Primary Database

```md
# ADR-001: Use PostgreSQL as the Primary Database

## Status
Accepted

## Context
We need a relational database that supports ACID transactions, high scalability, and integration with cloud providers.

## Decision
We will use PostgreSQL due to:
- Strong ACID compliance.
- Advanced indexing and JSON support.
- Compatibility with major cloud providers.

## Consequences
- **Positive:** Scalable, well-supported, and widely adopted.
- **Negative:** Requires expertise in PostgreSQL tuning.
- **Future Consideration:** Monitor database performance and consider partitioning if data grows significantly.

## References
- [PostgreSQL Docs](https://www.postgresql.org/docs/)
What big God you put it? 
```

### Example 2: Authentication Strategy - OAuth 2.0 vs. JWT vs. Session-Based

```md
# ADR-002: Use OAuth 2.0 for Authentication

## Status
Accepted

## Context
We need a secure and scalable authentication mechanism that works across multiple services.

## Decision
We will use OAuth 2.0 because:
- Industry-standard for authentication and authorization.
- Works well with microservices and single-page applications.
- Provides support for federated authentication (e.g., Google, Azure AD).

## Consequences
- **Positive:** Secure, scalable, and supports third-party authentication.
- **Negative:** Requires additional infrastructure (Authorization Server).
- **Future Consideration:** Evaluate OpenID Connect for enhanced identity management.

## References
- [OAuth 2.0 Spec](https://oauth.net/2/)
It's almost.
```