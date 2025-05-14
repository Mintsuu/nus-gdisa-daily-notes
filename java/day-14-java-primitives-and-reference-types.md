# Java Primitives & Reference Types 

## Reference types 
- Uses the memory address to point to the object 
- Memory address is saved, not the actual value 

## Primitive Types 
- Actually saves the value 

## Base Classes and Derived Classes 
- Subclasses inherit the states and behaviors from the superclass (subclass = child, superclass = parent)
- To instantiate the parent's class's constructor, use `super()`

## `protected` access modifier
- Variables/methods as part of the inheritance group is accessible (but has to be within the family tree)

## Method Overriding
- Child class can override the parent class's method using `@Override`
- Instead of overloading the parent class with methods that may be used in the child, probably better to use method overriding instead to keep the logic location consistent
- Can also verify that the method is supposed to override something (e.g. if the method that is supposed to override the parent method but it's misspelled, it will throw a runtime error)

## Static vs Non-static 
- Static methods/variables do not need the object to be instantiated to be used (e.g. a library of functions)
- Non-static methods/variables require the object to be instantiated to be used (e.g. class Animal)

## Questions 
- Is it common practice to set variables as `protected` so that those variables are accessible through the inheritance tree without the need to create getters and setters for those methods? And you can create getters and setter methods for variables that need to be accessed publicly (Can, but for now don't need to do any of that. Can read up more about "Information protecting")
- Is it possible to initialise class variables via the start of the class instead of creating a constructor to set the default values? (Can, but not best practice)
