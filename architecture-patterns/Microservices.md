# Microservices Architecture

- Distributed
- Separately deployable
- Service Components
- Boundary Context
- Data Domains
- API Layer
- Event Driven
- Reporting

*Microservices Architecture*

## Distributed Communication

- each service runs in its own process
- individually deployable
- sync
  - REST
  - RPC
  - HTTP
  - SOAP
- async
  - Messaging
  - Event Queues
- protocol-aware heterogeneus interoperability
  - service consumer
  - service provider
  - the caller needs to know the protocol of each service
    - protocol aware

## Separately deployable

- not only the services are separately deployable but also the infrastructure services
  - monitoring, logging
  - autorization, authentications
  - service discovery
  - service registry
  - api layer
- automated deployments
- elastic scale


*Microservices Elements***

## Service Components

- functional service
- infrastructure services
    - monitoring, logging
    - autorization, authentications
  - communication is point-to-point
  - api layer is optional
- messaging services
- point-to-point communication
- api layer is not a mediator
- a service component and background process
- service template
  - logging
  - monitoring
  - dropwizard.io
  - spring boot
  - coupling is bad
    - duplication is preferred to coupling
    - code that converts from JSON to XML is a code you want to share and a good example for a service template
  - authentication and authorization is another example

## Boundary Context

- what's the right size of a microservice?
- what's the purpose of the service?
- **transaction scope**, boundary, and context
  - business cases
  - we need a distributed transaction?
    - distributed transactions and rollbacks are hard
  - choreography
    - we need to coordinate with other services?
- microservices is a label, is not a description
- service scope and function
- single-purpose function
- purpose
- business process
- natural partitions in your system
- customer is not a boundary context
- catalog checkout is a boundary context
  - may include some customer information
- order management is a boundary context
  - may include some customer information
- payment is a boundary context
  - may include some customer information


## Service Orchestration
  
- no mediator

### Front Orchestrator


*Front Orchestrator*

- fire and wait?
- fire and forget

### Fire and Forget - Request Response


*Request Response*

- request response
  - update customer sends request to process quotes and wait for response
  

### Fire and Forget - Event Queue

- event queue
  - large data
  - more async behavior
  - no certainty
  - let the ending process consumes the messages and gather all the data
  - or let the ending process be the update customer process(the front orchestrator)
  - message queue
  - update customer sends request to process quotes and wait for response

*Event Queue*


*Service Orchestrator to Front Orchestrator*


*Service Orchestrator to Backend Process*

## Data Domains

- extremely level of granularity
- data domain
- brown field vs green field
- brown field and DBAs
  - existing data
  - existing processes
  - existing people
  - existing technology
  - existing tools
- we want to have a level of isolation, bundle some dbs, increase coupling
- assume low rate of schema changes or the usage of schemaless as nosql
  - schema changes can be risky
- reduces data duplication
- increases performance and reliability as transactions between services are reduced


*Data Domain*

## API Layer

- hides the actual endpoint of the service, exposing only those services available for public consumption
  - SPA that doesn't need to know the actual endpoint of the service and all the internal communication, elastic scale, service discovery, internal and external client requests
  - creates a facade for the service
  - feature toggles
  - rate limiting
  - monitoring
  - logging
  - security
- different APIs for different clients
- backend for frontend


*API Layer*


*API Layer - Backend for Frontend*


*API Layer - User Interface Layer*

### Proxies

- Apache HTTP Server
- Nginx
- HAProxy
- ZipProxy
- Proxy Server Squid
- IIS

### Load Balancers

- Barracuda
- f5
- Citrix Netscaler
- Neustar

## Gateway (Integration Hub)

General you don't to do too much of this, you don't want to too much coreography, orchestration, because of boundary context.

Important if you have to much integrations with external systems and legacy systems.

- Apache Camel
- MuleESB
- Kafka Streams

## Event Driven