# Refining Use Case Model 

## Steps 
- Extract common flow of work/tasks/activities from the use cases (do not go overboard)
- Find relationships such as 
  - Include relationships 
  - Exclude relationships 
  - Inheritance relationships

## Include Relationships 
- Essentially factor our common steps into a separate use case then use dotted arrow lines to re-insert the steps into the use cases that requires it
- Can have multiple relationships with the same inclusion
- Stop at 1 level instead of factoring too much 

## Generalisation of Actors 
- Arrow pointing: Child pointing to the parent (using OOP meaning)

## Abstract Use Cases 
- Exact steps to undertake the use case is different, but the end use case is the same (e.g. calling a local number vs calling an international number)
- 

## Extend Relationships 
- If a factored out use case has a condition to be executed, then it should be an extend relationship 
- Extend relationships are optional 


## Use Case Diagram Feedback
- Need to add login as a step (really from the very start)
- Can combine repeated processes into a procedure and make it into an entity (e.g. if every step requires GST calculation, can create a entity that "calculate GST price")
- 
