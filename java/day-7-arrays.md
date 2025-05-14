# Arrays

## How are arrays kept in memory
- Memory allocated is based on the data type
- Adjacent memory location is contiguously allocated for one word for each element in the array
- Important to declare size of array at the start
- 2D arrays depends on language, it's either a row wise or column wise allocation
- Arrays can have thousands of memory locations
- Computers use the index to locate the memory word using the start and offset

## Definition of Arrays
- Can store primitive values or objects
- Can only store fixed size of elements in array
- Java has anonyomous arrays

## Array Samples
```java

new int[]{1, 2, 3, 4, 5};
int[] fixedSizeArray = new int[5];
fixedSizeArray[0] = 10;
fixedSizeArray[1] = 20;
fixedSizeArray[2] = 30;
```

## Length
- Note that to check a string's length, you use the method `.length()`. To check an array's length, you use `.length`.
