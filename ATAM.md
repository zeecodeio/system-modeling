# ATAM (Architecture Tradeoff Analysis Method)
## What is it?
**ATAM** (Architecture Tradeoff Analysis Method) is a structured process for evaluating software architectures based on quality attributes and trade-offs.

## How to Perform ATAM?
1. **Define Business Goals** – Understand key drivers and constraints.
2. **Identify Architectural Approaches** – Document architectural styles, patterns, and tactics used.
3. **Map Quality Attributes** – Use the Utility Tree to assess the impact on security, performance, maintainability, etc.
4. **Analyze Trade-offs** – Identify which decisions benefit one attribute at the cost of another.
5. **Evaluate Risks & Sensitivities** – Highlight high-risk areas requiring additional validation.

## Example
If the system needs **high availability**, we might:
- **Use Multi-Region Deployment** → Improves **availability** but **increases cost & complexity**.
- **Cache with Redis** → Improves **performance** but **adds state management overhead**.
