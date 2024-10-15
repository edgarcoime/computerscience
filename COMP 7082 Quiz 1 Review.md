# Quiz 1 Review
## Week 1 - Agile Software Engineering
1. Plan Driven Development
2. Incremental Development 
3. Agile Methods:
	1. Scrum
	2. Kanban
	3. Extreme Programming
	4. Feature Driven Development
	5. Scaled Agile Framework
4. Key Scrum Practices
	1. Product Backlog
	2. Timeboxed Sprints
	3. Self-organizing teams
5. MoSCoW
	1. Must - A heart is a must
	2. Should - A hand is a should
	3. Could - Hair is a could
	4. Won't - unnecessary waste
## Week 2 - Features, Scenarios, and Stories
1. Feature List
2. Represent users using personas
	1. Dentist Appointment Management System: Dentist, Receptionist, Patient
3. Scenarios
	1. Narrative that describes how a user or group of users might use your system
	2. Avoid technical Details
4. User Stories
	1. Definition
	2. Content
	3. Standard Format
	4. Standard Format with Justification
5. User stories are used to describe features in the product that should be implemented
## Week 3 - Presentations
## Week 4 
1. What makes a good split
	1. Low coupling
	2. High Cohesion
	3. Abstraction and Encapsulation
2. Low coupling
	1. Coupling: How much interdependence along components in a program
	2. Before: A change in 1 part of the system leads to changes in many parts of the system
	3. After: The code is flexible and easier to maintain. Allows for changes in a part of the system without affecting others. 
3. High Cohesion
	1. Cohesion: Measure of strength/association of elements within component
	2. Problems of low Cohesion: Difficult to reuse and hard to maintain
	3. Benefits of high cohesion: Easy to maintain, reusability, testability, and single responsibility
4. Abstraction
	1. View of an object that focuses on relevent information and hiding implementation details
	2. Allows for interaction of an object without knowing internal details. 
	3. Problems Before: Too many details
	4. Benefits After: Simplified interface and easier to use
5. Encapsulation
	1. Grouping and packing internal details of an abstraction and making details inaccessible to external entities.
	2. Before encapsulation: no control and exposure of internal state
	3. Benefits after: controlled access and no unwanted access to internals
6. Class diagram
	1. Purpose: to show the static structure of the system in terms of classes and attributes
	2. Visibility: Sets accessibility of attribute and methods
	3. Multiplicity: Indicating n to j relationships between entitites
	4. Aggregation (Has-a relationship)
		1. Parts exist independent of the whole
		2. Team has multiple players
		3. But if team is dissolved players don't disappear as well
	6. Composition (Has-a but stronger relationship)
		1. Parts are destroyed when the whole is destroyed
		2. A house has many rooms
		3. If the house is destroyed the rooms are destroyed along with it
	7. Generalization
		1. Labelled group of generalizations with a common superclass
		2. habitat -> Aquatic, Land
		3. Type of Food -> Carnivore, Herbivore
	8. Association
		1. No specific dependencies just a basic association relationship
		2. SeaAnimal --- SeaUrchin
			1. Eats
7. Sequence Diagrams
	1. Type of diagram that illustrates how objects or classes within a system interact over time 
	2. Shows interaction as they take place and how classes collaborate with one another. 
	3. Steps
		1. Identify Actor and Objects
		2. Lifelines
		3. Messages and interactions
		4. Alternative frames for conditional logic
		5. Activation Boxes
8. State Diagram
	1. Technique used to describe how a system behaves or responds to events
	2. Has 3 main components: 
		1. State Name
		2. State Variables
		3. State Activities
	3. Benefits: 
		1. Visualize object behaviour
		2. Error detection or missing conditions
		3. Testing
## Week 5 
1. Architectural trade-offs
	1. Maintainability
		1. Decompose app into fine-grain components
		2. Small, compact, and easy to maintain
		3. Easy to test and can easily find parts that can be reusable 
	2. Communication Overhead (Performance)
		1. More components introduces more communication between them which in turn means added latency
2. ORMS vs SQL queries
	1. Easy to maintain, low performance *
		1. Relatively low performance compared to raw sql
		2. Easy to maintain and even swap out DBMS down the road since interop is abstracted out
		3. Faster development times because usually easier than designing raw sql queries
	2. Hard to maintain, higher performance
		1. High performance and can leverage specific dbms features to be more efficient
		2. Hard to maintain and now query structure responsibility is now pushed onto the developers
3. Centralized security architectures
	1. Easier to design and build protection but if security is breached lose everything
	2. Security
		1. Achieve security by having multiple layers that an attacker has to go through
		2. Auth layers, critical feature auth layer, and may encryption layer
	3. Usability
		1. Layered approach makes your codebase harder to onboard and get used to especially when switching teams.
		2. On the users point of view if there are too many security checks they can get irritated and they will always find ways to make it easier to login
4. Availability vs time-to-market
	1. Refers to percentage of time that the system is up and running and delivering service to users
	2. Very important for certain industries such as banking and government
	3. Can be achieved by introducing redundant component
		1. Coupled with sensor components to detect failure
	4. Increased development time and complexity
5. Architectural Design decision issues
6. Architectural Complexity
7. Technology Choices
	1. Database: SQL vs ORM
8. Delivery Platform
	1. Mobile
	2. Web-based
9. Server considerations: Cloud vs Customer Serves
10. Toolchain
	1. OSS
## Week 6 
## Week  7