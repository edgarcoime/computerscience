## Software Modeling
1. We need to represent our working system in an abstract way
2. Two types of modeling:
	1. Structure Models:
		1. Class diagrams, Entity-Relationship diagrams
	2. Behavioural modeling:
		1. Use case Diagrams, Sequence Diagrams, State Diagrams
### Class diagrams
1. Are used when developing an object-oriented system model to show the classes in a system and the associations between these classes. 
2. The purpose is to show the static structure of the system in terms of classes and attributes, operations and relationships.
3. Visibility
	1. - private
	2. + public
	3. # protected 
	4. ~ package (any other class as long as in the same package)
4. Multiplicity
	1. Symbols indicating multiplicity are shown at each end of the association
	2. 0..1 zero to one
	3. n specific number
	4. 0..* zero to many
	5. 1..* 1 to many
	6. m..n specific range
5. Composition
	1. A strong type of aggregation 
6. Generalization
7. Association
	1. No specific dependencies, just a basic association relationship
### Sequence Diagrams
1. Only diagram that captures time passing and how objects and classes interact with the system over time 
2. Example: ATM system
	1. Actors - External entities in the system that interact with your system
	2. Objects
		1. ATM
		2. Bank Server
		3. Bank Account