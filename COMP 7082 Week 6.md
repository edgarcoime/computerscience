# Architectural patterns
## Layered Pattern
1. defn: Separation of concerns among component
	1. Data - database (postgres)
	2. Persistent layer - database service, orm, or database conn class
	3. Service layer 
		1. In this case it is acceptable for the business logic layer to skip over services and go straight to persistent layer. 
	4. Business logic - API
	5. Presentation layer - Web client / desktop app
2. Layered patterns provides a separation of concerns
	1. Each layer can function independently (isolated) from one another 
3. Cross-cutting concerns
	1. Concerns that affect all layers of the system architecture
		1. Issues that all layers have to deal with and handle
	2. Some examples: 
		1. Security
		2. Performance
		3. Reliability
4. How do we handle these concerns?
5. Aspect-oriented programming
	1. Aspect: A module that encapsulate the desired behaviour
	2. Joint Point: A point in the program where the "aspect" can be applied such as method execution or instantiation
	3. Advice: Aspect code that is executed at joint point should be before, after, or around.
	4. Pointcut: A set of join points where an advice should be applied. 
6. Pros
	1. Allows for the replacement of entire layers as long as the interface is maintained
7. Cons
	1. Designing the system architecture to only interact with the layers below it is hard and at times and higher level layers may interact with lower levels directly instead of the layers between them.
	2. Performance can be a problem especially if multiple layers are involved
## Monolithic Pattern
## Client Server
1. Distribution architecture that is suited for applications that share a database and business logic
2. Client: 
	1. The application/presentation layer aspect of the system that users insteract with
3. Server: 
	1. The business logic layer of the system that interacts with the database
4. Load Balancer:
	1. Responsible for distributing incoming network traffic across backend servers to update resource usage
5. Examples: 
	1. Internet
	2. DNS
		1. Server that maps ip-addresses to human readable strings
		2. Does not communicate through http but rather through dns protocol or udp
## Model View Controller
1. MVC design pattern separates application into three main components:
	1. Model
	2. View
	3. Controller
2. Pros
	1. Seperation of concerns
	2. Parallel development
	3. Reusability
	4. Testability
3. Cons:
	1. Tight coupling between controller and view
	2. Difficulty in managing many views
## Event Driven Architecture
1. Mainly used in Distributed asynchronous architecture pattern
	1. Highly scalable
	2. Made of highly decoupled single purpose event processing compartments
2. 2 main strategies
	1. Mediator
	2. Broker
3. Architecture components:
	1. Event queues
	2. Event mediator
	3. Event channels
	4. Event processors
## Repository Pattern
1. A sharing data pattern in a star pattern
2. Sub systems must exchange data. This may be done in two ways:
	1. Shared data is held in a central database or repository and may be accessed by all sub-systems
	2. Each sub-system maintains its own database and passes data explicitly to other sub-systems
## Pipe and filter pattern
## Service Oriented Architecture
## Quiz
1. Software Products
2. Features, Scenarios, and Stories
3. 