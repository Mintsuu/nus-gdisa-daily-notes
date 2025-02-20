# Classes and Objects 
## Classes 
- A blueprint that models a real-world entity 
- Defines:
  - Attributes (data) of objects 
  - Methods (logic) to manipulate the attributes
- `objects` are instances of a `class` 
- Each Java `class` resides in a separate file of its own 
- Java compiles the code into Java Byte Code (a `Java Byte Code in a .class file extension`)
- The resulting `byte code` then runs on a `Java Virtual Machine` 
```
class Person {
  private String name = "";
  private int age = 0;
  private boolean gender = false;
  private double height = 0.0;

  public static void intro() {
    // Introduce self
  }
}
```
## The `.this` variable (Scope)
- `this` references current object and used to access instance variables within the class

## The `Constructor` Method 
- A special `method` that is automatically executed upon object creation
- Needs to be public or else the class won't be able to instantiate a new object

## Arrow Methods (or aka `Lambda` functions in Java)
- Instead of using `() => {}` in `javascript`, `java` uses `() -> {}`
- Seems to work just like how it works in `javascript`

## Access Modifiers
- `public`
  - Allows attribute/method to be read and updated from **outside its class**
  - Allows method to be invoked from **outside its class**
- `private`
  - Only readable from **within the class**
  - Methods can only be invoked by the **class**
- `protected`
- Used to control external access to attributes and methods of a class
- Have no effect within the class
- 

## Function Overloading
- Allows a class to have constructors and methods of the same name, as long as parameters are different


