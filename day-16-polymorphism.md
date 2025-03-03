# Polymorphism
## Object References
- There are 3 steps in object instantiation and assignment 
  - Create an object `new Cat()`
  - Declare reference variable `Cat myCat`
  - Assign the reference variable to the object `Cat myCat = new Cat();`

## References 
- Child class can be instantiated with parent class type 
- E.g. `Animal newCat = new Cat();` means the variable is of type `Animal`, but it's assigned to `Cat`
- In neural language, an animal can be a cat, but a cat may not be an animal. Therefore `Cat newCat = new Animal();` is invalid 
- Seems like the `type` fully defines what methods the object may have. It may be instantiated with a different object but the type defines what is allowed and what isn't
- Reference type (the type of the variable) determines what methods can be called. Object type is the assigned type. 
- The executed methods will stem from the object type (aka the object that it was instantiated on)

## Interface 
- Interface is a collection of methods 

## Polymorphic Arrays/Collections 
- Able to create an array out of multiple child classes true

```java
Animal[] myAnimals = new Animal[4];
myAnimals[0] = new Cat();
myAnimals[1] = new Cow();
myAnimals[2] = new Pig();
myAnimals[3] = new Cow();
```
```
```java
Animal myCat = new Cat();
myCat.makeNoise();
// Animal's methods will be inherited
// But Cat.makeNoise() will be invoked
```

## Questions
- How do you access the class's grandparent inherited properties? (You are not able to. This is usually an indicator that your architecture design is profoundly wrong)
