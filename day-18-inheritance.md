## ArrayList vs Array 
- Faster to use Arrays 
- ArrayList is dynamic size 

## ArrayList
- Is a class type `ArrayList`
- Usually empty constructor, but it accepts a `Collection` to initialise the ArrayList (to look into this)

## HashMaps 
- Is a class type `HashMap`
- Can set generic key and value 

## Abstract Methods 
- No implementation, but child classes *must* create the method

## Interfaces 
- Basically same as typescript
- Any class that `implements` an interface is required to supply all the methods of the interface without question 
- A class can implement multiple interfaces 

## Questions 
- When do you use an empty implementation with an @Override method in the child class vs abstract methods? (The child method cannot be successfully created if it does not meet the criteria of the abstract methods defined in the parent class)
- Can you do method overloading with abstract methods? (Can, it just acts like any other method, but provides instructions to the child class)
- Instead of using the direct `protected` attributes from the parent, is it best practice to use `super.color = "red"` instead
- Do you usually store all interfaces in a package of its own? 

