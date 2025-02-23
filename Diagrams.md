# Diagrams

## [The C4 model](https://c4model.com/)

See also [likec4](https://likec4.dev/)

### System Context

Context Diagram: Present a high-level diagram (macroarchitecture) of the application following the C4 model. 

> Draw a diagram showing your system as a box in the centre, surrounded by its users and the other systems that it interacts with.
> C4 Model

### System Containers

Container Diagram: Present a diagram of repositories (containers) and their components.

> Once you understand how your system fits in to the overall IT environment, a really useful next step is to zoom-in to the system boundary with a Container diagram. A “container” is something like a server-side web application, single-page application, desktop application, mobile app, database schema, file system, etc. Essentially, a container is a separately runnable/deployable unit (e.g. a separate process space) that executes code or stores data.
> The Container diagram shows the high-level shape of the software architecture and how responsibilities are distributed across it. It also shows the major technology choices and how the containers communicate with one another. It’s a simple, high-level technology focussed diagram that is useful for software developers and support/operations staff alike.
> C4 Model

### System Components

Component Diagram: 

> Next you can zoom in and decompose each container further to identify the major structural building blocks and their interactions.
> The Component diagram shows how a container is made up of a number of “components”, what each of those components are, their responsibilities and the technology/implementation details.
> C4 Model


### Dynamic View

This diagram presents use cases, user story, features interaction - journeys, flows, user journey, similar to Dynamic UML diagrams as Sequence, Communication, Activity, State, ...;

> A dynamic diagram can be useful when you want to show how elements in the static model collaborate at runtime to implement a user story, use case, feature, etc. This dynamic diagram is based upon a UML communication diagram (previously known as a “UML collaboration diagram”). It is similar to a UML sequence diagram although it allows a free-form arrangement of diagram elements with numbered interactions to indicate ordering.


### Deployment View

This diagram presents how and where the artifacts are deployed over the underline infrastructure as well some fudamentals interactions between artifacts and infra;

>A deployment diagram allows you to illustrate how instances of software systems and/or containers in the static model are deployed on to the infrastructure within a given deployment environment (e.g. production, staging, development, etc). It’s based upon a UML deployment diagram.
> A deployment node represents where an instance of a software system/container is running; perhaps physical infrastructure (e.g. a physical server or device), virtualised infrastructure (e.g. IaaS, PaaS, a virtual machine), containerised infrastructure (e.g. a Docker container), an execution environment (e.g. a database server, Java EE web/application server, Microsoft IIS), etc. Deployment nodes can be nested.
> You may also want to include infrastructure nodes such as DNS services, load balancers, firewalls, etc.
> Feel free to use icons provided by Amazon Web Services, Azure, etc to complement your deployment diagrams … just make sure any icons you use are included in your diagram key/legend.
> C4 Model
