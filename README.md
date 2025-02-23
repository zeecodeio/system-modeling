# System Modeling

Open to changes and collaborations; WIP

## References

- PUC Minas - Arquitetura de Software Distribuido | Distributed Software Architecture
- Neal Ford
- Mark Richards
- Simon Brown
- Chris Richardson
- Fábio Aguiar
- Paulo Caroli
- ChatGPT and Claude.ai(reviewed but still may have some hallucinations (⌒_⌒;))
- ...

## 1. Introduction

Work Contextualization: Describe the project, its area or context, and the problem it aims to solve, including its motivation.

This section presents the context, problem, and objectives of this work. It should begin with a brief description of the business area and its significance, followed by an introduction to the work's subject matter.

### Context

In the initial section (contextualization), the context/scope addressed in the work should be presented, including the broader area or context it belongs to and why it is important. The contextualization should be developed from the general/generic to the particular/specific. Citing research with quantitative data properly referenced is highly recommended. The referenced study should be similar, at least in part, to the work you are developing.

In this phase, you may need to spend some time modeling the business, actors, and personas.

### Problems Statements

List and describe the problems that the solution is trying to solve;

In this section, the Architect has to create an explanation of each problem. The problem must be presented succinctly, comprehensively, and clearly, as understanding it is essential to developing a proposed solution. The problem description does not indicate how it will be solved or suggest a solution. It represents the so-called "customer pain point."

### Motivations

What are the motivations for solving the problems? This motivation can take various forms: academic, market-driven, social, etc. This section serves to justify the work by highlighting the importance of undertaking it. Avoid using personal motivations, as they are irrelevant here. Including expected results and/or quantitative data at this point is also a good practice. For example, benefits such as resource savings, faster decision-making, improved process quality, etc., can be highlighted.

### Objectives | Expectations | Goals

List the main objectives, expectations, and goals you're trying to achieve;

Present the general objective and at least three specific objectives. These definitions will demonstrate the overarching/final goal related to your architectural description and how it can be achieved through partial goals.

## Business Model

Add more details about the business related to the system;

## 2. Personas

Describe the personas that will interact with the solution, their problems, what the person does, their activities, and what're their expectations;

## 3. User Journeys

[**User Journey**](./User-Journey.md) describes the end-to-end experience of a user interacting with the system. It helps visualize the flow of actions users take to achieve their goals, highlighting pain points, key interactions, and moments of delight.

## 4. Architectural Specification of the Solution

This section presents the basic specification of the solution's architecture, including diagrams, constraints, and requirements defined by the author. This allows for a clear visualization of the solution's architecture.

### Constraints

List the architectural constraints related to your project here. Remember that architectural constraints are generally not considered requirements, as they limit the candidate solution but do not constitute functionalities or needs to be fulfilled. In other words, unlike requirements, they impose restrictions that must necessarily be satisfied.

Architectural Constraints: Describe the constraints related to the chosen scope, things like frameworks, programming languages, platforms, etc;

| ID  | Description |
| --- | ----------- |
| C1  |             |

### Functional Requirements | Functionalities

List all the functional requirements planned for your application. Include all the requirements to ensure architectural coverage according to the provided specifications. This section should contain a comprehensive list of requirements to produce a complete model of the solution.

Functional Requirements: List and briefly describe the application's functional requirements, prioritizing them. If necessary, organize the requirements by modules.
Note: This document does not require an exhaustive and detailed description of the requirements. A summarized description with numbered items for better identification is sufficient.

**F**URPS+

Functionality

Describe the main functionalities of the system, contextualize the actions around the personas describe the problems it's solving and the benefits it's creating for the person;

| ID    | Summarized Description | Difficulty (L/M/H) | Priority (L/M/H) |
| ----- | ---------------------- | ----------------- | ----------------- |
| FR01  |                        |                   |                   |

### Non-functional Requirements | Quality Attributes

List all the non-functional requirements planned for your application. Include all requirements deemed necessary from an architectural perspective, i.e., those that will impact the definition of the architecture. The requirements should be described comprehensively and preferably quantitatively (e.g., response time of "x" seconds).

Non-Functional Requirements: Include all non-functional requirements deemed necessary from an architectural perspective, particularly those impacting the solution proposal.

F**URPS+**

Usuability, Reliability, Performance, Security, +

| ID    | Summarized Description | Priority |
| ----- | ---------------------- | -------- |
| NFR01 |                        |          |

- [Trigger List for Non-Functional Requirements](Non-Functional-Requirements-Trigger-List.md)

### Architectural Mechanisms

[Architectural Mechanisms](Architectural-Mechanisms.md): Describe the mechanisms that bridge the conceptual definition of the solution (analysis) and its implementation, transitioning through the design perspective.

This section provides an overview of the mechanisms that make up the software architecture based on three stages: **Analysis**, **Design**, and **Implementation**.

#### 1. Analysis
List the general aspects that compose the software architecture, including:
- **Persistence**: Data storage and retrieval mechanisms.
- **Integration**: Interaction with legacy systems.
- **Logging**: System log generation and management.
- **Front-End Environment**: Frameworks and tools for the user interface.
- **Exception Handling**: Strategies for managing errors and failures.
- **Testing Format**: Approach and structure for software testing.
- **Deployment Format**: Distribution and deployment methods for the solution.
- **Code Collaboration and Integration**
- **Infrastructure Provisioning**
- **Disaster Recovery**
- **Lead Time**
- **Delivery Throughput**
- **Observability**

#### 2. Design
Identify the technological patterns to follow for each mechanism identified in the **Analysis** phase.



#### 3. Implementation
Specify the products or tools to be used in the solution, assuming it were to be implemented.

| Analysis    | Design                | Implementation            |
| ----------- | --------------------- | ------------------------- |
| Persistence | • Relational DB       | • Postgres                |
|             | • ORM                 | • Spring Data/Hibernate   |
| Backend     | • N-Layer             | • Spring Boot             |
|             | • Java DTOs           | • Lombok                  |
|             | • External Config     | • Spring Profile          |
|             | • Health Checks       | • Spring Actuator         |
| Frontend    |                       |                           |
| Integration |                       |                           |
| Security    |                       |                           |
| Logging     |                       |                           |
| Testing     |                       |                           |
| DevOps      |                       |                           |
| Monitoring  |                       |                           |

- [Trigger List for Architectural Mechanisms](Architectural-Mechanisms-Trigger-List.md)

## 5. System Architecture

### Diagrams

Use 4+1 View and C4 Model [diagrams](./Diagrams.md)


### Create a Utility Tree

A [**Utility Tree**](./Utility-Tree.md) is a hierarchical structure that captures the system's key **quality attributes** (e.g., performance, security, scalability) and breaks them down into measurable scenarios.

### Document Initial ADRs

[**Architectural Decision Records (ADRs)**](./ADR.md) document key decisions made about system design, ensuring historical context and rationale are preserved.

## 6. Architectural Analysis

[**Architectural Analysis**](./Architectural-Analysis.md) is the process of evaluating software architectures to ensure they meet business and technical requirements. Various methodologies exist to analyze trade-offs, assess risks, and determine how well the system meets its quality attributes.


## Links

- [Architectural Mechanisms](Architectural-Mechanisms.md)
- [Architectural Mechanisms Trigger List](Architectural-Mechanisms-Trigger-List.md)
- [Architectural Requirements](Architectural-Requirements.md)
- [Checklists](Checklists.md)
- [Guides](Guides.md)
- [Non-Functional-Requirements-Trigger-List](Non-Functional-Requirements-Trigger-List.md)
- [Requirements Checklist](Requirements-Checklist.md)
- [Architectural Patterns](Architecture-Patterns.md)
 
