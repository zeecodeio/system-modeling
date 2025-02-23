# Create a Utility Tree
## What is it?
A **Utility Tree** is a hierarchical structure that captures the system's key **quality attributes** (e.g., performance, security, scalability) and breaks them down into measurable scenarios.

## How to Create It?
1. **Define High-Level Quality Attributes** – These could be **performance, scalability, maintainability, availability, usability, security**, etc.
2. **Break Down into Specific Scenarios** – Define sub-attributes and concrete use cases for each.
3. **Prioritize** – Rank attributes by importance to stakeholders.
4. **Evaluate Risks** – Identify challenges in achieving these qualities.

## Example
For an **E-commerce System**, the utility tree could look like this:

- **Performance**
  - Page load time < 2s under 1,000 concurrent users.
  - API response time < 100ms for critical endpoints.
- **Security**
  - Encrypt sensitive user data (AES-256).
  - Implement OAuth2 for authentication.
- **Scalability**
  - Handle 10,000 users per minute with auto-scaling.
- **Maintainability**
  - Microservices should have less than 10% interdependency.