# Realising Use Cases
## Making a sequence diagram
- Only needs 1 controller 
- Name the controller as the use case name 
- 3 main components
  - Boundary: Interface for actors to use (necessary when the sequence diagram is relating to the actor)
  - Entity: The name of the entity that's referenced to in the use case 
  - Controller: Main tool that orchestrates the entire flow of the program
- Only need to define attributes for entities, let programmers decide what attributes is required for the controllers and boundaries 

## Flow of system architecture
- 

## Relationships 
- ..> Dependency (client - supplier relationship, temporary relationship)
  - RentCarController ..> BillingSys (RentCarController only needs to access BillingSys temporarily)
- --> Association (structural relationships, permanent relationship)
- o--> Aggregration (Part + whole relationship)
- *--> Composition (Lifetime of part-whole relationship)
- --|> Inheritance (is-a relationship)
## Restrictions 
- Entities **cannot** interact with boundaries (huge error in design, and is a common mistake in exams)
- Entities can have a relationship with itself 

