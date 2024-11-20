# FURPS+

> [System Modeling](README.md)

- Functionality
- Usability
- Reliability
- Performance
- Supportability

The "+" in FURPS+ also helps us to remember requirements such as:
- Design requirements
- Implementation requirements
- Interface requirements
- Physical requirements 
## Functionality
The Functionality category of the FURPS+ classification gathers all functional requirements. These requirements generally represent the main product features. In a warehouse application, we might have requirements pertaining to "Order Processing" or "Stock Control". 

However, functional requirements are not always domain-specific. For example, providing printing capability is a functional requirement of particular significance to architecture. The remaining "URPS" categories are used to describe nonfunctional requirements, which are also generally of architectural significance.
## Usability
Usability is concerned with characteristics such as aesthetics and consistency in the user interface.

- Accessibility (e.g. the system supports IE, Chrome browsers)
- Consistency (e.g. all error messages look the same throughout the system)
- Navigation rules (e.g. it concerns the support of using the keyboard, mouse or keyboard shortcuts)
- Training time (e.g. the training of new users will take 2 days or 8 hours)
- Usability standards (e.g. the usability solution will be in line with company policy/standards)

| **Usability Requirement**  | **Description**                                                                                                |
|----------------------------|----------------------------------------------------------------------------------------------------------------|
| **Accessibility**          | The ease with which different facets of the system are exercised.                                              |
| **Aesthetics**             | The aesthetic quality of the user interface.                                                                   |
| **Consistency**            | The consistent use of mechanisms employed in the user interface, both within the system and with other systems.|

**Architectural Requirement Questionnaire**

| **Requirement**    | **Questions**                                                                                         | **Impact**                                                                                     |
|---------------------|------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------|
| **Accessibility**   | - Are there any special requirements that relate to the ease with which the system can be exercised (including a novice user)? | The greater the accessibility, the longer the time to market, and the greater the long-term maintenance cost. |
| **Aesthetics**      | - Are there any special requirements regarding the "look and feel" of the system?                    | The greater the aesthetic appeal, the longer the time to market.                              |
| **Consistency**     | - Are there any special requirements regarding the consistency of the user interface, both within the system, and with other systems? | The greater the level of consistency, the longer the time to market.                          |


## Reliability
Reliability is concerned with characteristics such as availability (the amount of "up time" of the system), accuracy of calculations
performed and recoverability of the system from failure.

| **Requirement**    | **Description**                                           |
| ------------------ | --------------------------------------------------------- |
| **Accuracy**       | The accuracy of any calculations performed.               |
| **Availability**   | The amount of "up time" of the system. Uptime, MTBF, MTTR |
| **Recoverability** | The elegance with which the system recovers from failure. |

**Architectural Requirement Questionnaire**

| **Requirement**   | **Questions**                                                                                     | **Impact**                                                   |
|--------------------|--------------------------------------------------------------------------------------------------|-------------------------------------------------------------|
| **Accuracy**       | - Are there any particular constraints on the accuracy of any calculations to be performed by the system? | The greater the level of accuracy, the longer the time to market. |
| **Availability**   | - Are there any requirements regarding system "up time"? This may be specified in terms of Mean Time Between Failures. | The higher the availability, the longer the time to market.  |
| **Recoverability** | - Are there any special requirements regarding recovery from a system failure?                   | The greater the level of recoverability, the longer the time to market. |


## Performance
Performance is concerned with characteristics such as throughput, response time, recovery time, start-up time and shutdown time.

- Capacity (e.g. the system must store 5 TB of data)
- Throughput (e.g. the system must support 100k transactions per minute or the system must support the parallel operation of 200 users)
- Response time (e.g. the system must respond in a maximum of 2 seconds, the maximum login time cannot be longer than 1 second)
- Scalability (e.g. that the system must automatically scale)

| **Performance Requirement**  | **Description**                                                                                                                              |
|------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------|
| **Response Time**            | The time for the system to provide a response.                                                                                               |
| **Processing speed**         |                                                                                                                                              |
| **Latency**                  | Latency is a time delay between the cause and the effect of some physical change in the system being observed                                |
| **Channel capacity**         | Channel capacity is the tightest upper bound on the rate of information that can be reliably transmitted over a communications channel.      |
| **Start-up Time**            | The time for the system to start up.                                                                                                         |
| **Throughput**               | The capacity of the system to support a given flow of information, is the rate of production or the rate at which something can be processed.|                                            |

**Architectural Requirement Questionnaire**

| **Requirement**    | **Questions**                                                                                     | **Impact**                                                                                  |
|---------------------|--------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------|
| **Response Time**   | - Are there any constraints on the time taken for the system to respond to particular events, such as user interaction? | The shorter the response time, the longer the time to market.                              |
| **Start-up Time**   | - Are there any requirements on the time taken to start the system?                              | The shorter the start-up time, the more sophisticated the start-up mechanism and the longer the time to market. |
| **Throughput**      | - Are there any special requirements regarding throughput of data supported by the system?       | The greater the throughput of data, the longer the time to market.                          |


## Supportability
Supportability is concerned with characteristics such as:

- testability, 
- adaptability, 
- **maintainability**, 
- compatibility, 
- configurability,
- installability, 
- scalability 
- and localizability.

| **Requirement**     | **Description**                                                                            |
|----------------------|--------------------------------------------------------------------------------------------|
| **Adaptability**     | The ease with which the system is adapted to new environments.                             |
| **Auditability**     | The ease with which the system provides audit trails of its execution.                     |
| **Compatibility**    | The compatibility of this system with previous versions of the system.                     |
| **Configurability**  | The ease with which the system is configured.                                              |
| **Installability**   | The ease with which the system is installed.                                               |
| **Localizability**   | The level to which the system supports multiple human languages.                           |
| **Maintainability**  | The ease with which the system is maintained.                                              |
| **Scalability**      | The ease with which the system can scale in terms of data volumes and users.               |
| **Testability**      | The ease with which the system is tested.                                                  |

**Architectural Requirement Questionnaire**

| **Requirement**    | **Questions**                                                                                     | **Impact**                                                                                  |
|---------------------|--------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------|
| **Adaptability**    | - Are there any special requirements regarding the adaptation of the software (including upgrading)? | The greater the adaptability of the system, the longer the time to market, and the greater the long-term maintenance cost. |
| **Compatibility**   | - Are there any requirements regarding this system and its compatibility with previous versions of this system or legacy systems providing the same capability? | The greater the compatibility, the longer the time to market.                              |
| **Configurability** | - Will the product be configured after it has been deployed? <br> - In what way will the system be configured? | The greater the configurability of the system, the longer the time to market, and the greater the long-term maintenance cost. |
| **Installability**  | - Are there any special requirements regarding system installation?                              | The greater the installability of the system, the longer the time to market.               |
| **Maintainability** | - Are there any special requirements regarding system maintenance?                               | The greater the maintainability of the system, the longer the time to market. The trade-off is between time to market of the first release of the system, and any subsequent releases. |
| **Scalability**     | - What volumes of users and data will the system support? <br> - This may be expressed as a profile over time. | The greater the scalability of the system, the longer the time to market.                  |
| **Testability**     | - Are there any special requirements regarding the testability of the system, such as testing "hooks" that allow integration with a testing tool? | The greater the testability of the system, the longer the time to market.                  |

## Design Requirement | Constraints

A design requirement, often called a design constraint, specifies or constrains the design of a system. For example, it might be
stated that a relational database is required. This is a design constraint – it constrains our design options.

A design requirement is simply a constraint on the refinement of an analysis mechanism, such as those listed in –
**Analysis mechanism**. For example, a requirement for a relational database is a constraint on the refinement of a persistence
analysis mechanism. The set of design requirements to consider is therefore derived directly from the list of analysis mechanisms.

**Architectural Requirement Questionnaire**

All design requirements are addressed in the section titled "Analysis mechanisms".


## Implementation Requirement
An implementation requirement specifies or constrains the coding or construction of a system. Examples might include required standards, implementation languages and resource limits.

| **Implementation Requirement** | **Description**                                                             |
|---------------------------------|-----------------------------------------------------------------------------|
| **3rd Party Components**        | Any constraints on the use and cost of third-party components.             |
| **Implementation Languages**    | The implementation languages to be used.                                   |
| **Platform Support**            | The platforms that the system will support.                                |
| **Resource Limits**             | Limits on the use of resources such as memory and hard disk space.         |
| **Standards-Compliance**        | Any standards to which the system must conform.                            |

**Architectural Requirement Questionnaire**

| **Requirement**            | **Questions**                                                                                                           | **Impact**                                                                                                                                                                       |
|-----------------------------|------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **3rd Party Components**    | - Are there any constraints (including cost) on the use of 3rd party components in the system? <br> - How important is it for the system to be vendor-independent, in terms of the 3rd party components it uses? <br> - Are there any approved relevant alliances with 3rd party vendors? | The more 3rd party components used, the shorter the time to market. <br> Existing alliances typically remove the need for contractual negotiations, improving the time to market. |
| **Implementation Languages**| - Are there any constraints on the programming languages used to develop the system?                                   | Specification of particular programming languages must align with tool support and available skills. If tools or skills are unavailable, time to market increases.               |
| **Platform Support**        | - What platforms must the system support? <br> - Which operating system versions must be supported? <br> - Is web access required? <br> - Which web browsers and versions must be supported? <br> - Is it anticipated that the system will be ported to new platforms in the future? | Development for a single platform shortens the time to market and allows closer integration with platform features. Development for multiple platforms lengthens time to market but eases deployment on new platforms. |
| **Resource Limits**         | - Are there any limits on the use of system resources, such as memory or hard disk space?                              | The more constrained the available resources, the more efficient resource use is required, which increases time to market and reduces maintainability.                          |
| **Standards-Compliance**    | - Are there any standards to which the system must conform? <br> - Does this include coding standards or a user interface style guide? | Use of available standards can decrease time to market and improve consistency across multiple areas of the system.                                                             |

## Interface Requirement
An interface requirement specifies or constrains the interfaces between components. Examples might include required protocols, data formats and interfaces.

| **Requirement**        | **Description**                                                       |
|-------------------------|------------------------------------------------------------------------|
| **External Systems**    | External systems with which this system must interface.               |
| **Interface Formats**   | The format of any data passed between this and external systems.      |

**Architectural Requirement Questionnaire**

| **Requirement**      | **Questions**                                                                                                    | **Impact**                                                                                                     |
|-----------------------|-----------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------|
| **External Systems**  | - Are there any external systems with which this system must interface? <br> - Consider both provided and required interfaces. | The greater the sophistication of the interface to external systems, the longer the time to market, and the greater the long-term maintenance cost. |
| **Interface Formats** | - Are there any constraints on the nature of the interface between this system and any external system? <br> - Does this include the format of data passed between these systems, and any particular protocol used? | The greater the sophistication of the format of interfaces, the longer the time to market, and the greater the long-term maintenance cost.         |

## Physical Requirement
A physical requirement specifies or constrains the physical properties of a system. Examples might include required hardware, installation locations and environmental conditions.

| **Physical Requirement** | **Description**                                            |
|---------------------------|-----------------------------------------------------------|
| **Shape**                 | The shape of the resulting hardware housing the system.   |
| **Size**                  | The size of the hardware housing the system.              |
| **Weight**                | The weight of the hardware housing the system.            |


## Examples

- "The product will be localized" is a supportability requirement.
- "The persistence will be handled by a relational database" is a design requirement.
- "The database will be PostgreSQL" is an implementation requirement.
- "The system will run 7 days a week, 24 hours per day" is a reliability requirement.
- "An online help system is required" is a functional requirement.
- "All presentation logic will be written Java Spring Boot" is an implementation requirement. 
