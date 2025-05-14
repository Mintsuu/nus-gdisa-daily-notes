## Java Autobox
- Converts primitive types into their object wrapper class (e.g. `int` to `Integer`)

## Comparison between generics
- There is a built in generic interface `Comparable<T>` that has a `.compareTo()` method that is built in with most native classes in Java 
- Can extend generic types with this interface to compare between generics 

## Generics 
- T is usually short for type 
- E is usually short for element

## Functional Programming 
### Lambda Functions 
- If a lambda function doesn't return anything and only calls another function, can use `ClassName::methodName` e.g. `System.out::println("Hello world")`
```
E.g. 
int compare(Person a, Person b) {
return a.compareByAge(b);
}

|
v 

(a,b) -> a.compareByAge(b) 

|
v 

Person::compareByAge
```
- Lambda functions have to be specifically typed properly e.g. `Function<C, R> sum = (a) -> a`
- Oddly enough, variable number of parameters can't be used with the generic `Function` type
- Have to use `BiFunction` instead and declare the input and return types properly 

## Streams 
- A collection of methods to perform on a collection 
- Convert the collection into a stream before doing anything 
```
e.g. 
int[] arr = {3,10,2,4,0};
IntStream.of(arr)

Integer[] arr = {};
arr.stream()...
```
