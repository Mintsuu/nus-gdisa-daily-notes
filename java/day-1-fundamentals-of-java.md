# Fundamentals of Programming with Java

by Liu Fan

## Typical Daily Schedules

- Quizes
- In-class Discussions
- Lectures
- Workshop and Exercises

### Grading

- Paper 1 - Design (SA4101)
- Paper 2 - Foundation (SA4105), cinludes FOPJ, OOPJ, etc
- 20-25% of Term 1 Paper Technical Subject Grade is from FOPJ
- In class exercises not graded
- Writing code in exams (logic errors and structural errors will be penalized)

### Java References

- Oracle Java Website: https://www.oracle.com/java/
- Java Tutorial: https://www.tutorialspoint.com/java/index.htm
- "Java: A beginner's Guide", 8th Edition, Herbert Schildt
- "Effective Java", 3rd Edition, Joshua Bloch, 2017
- "Introduction to Java Programming", Y. Daniel Liang, latest edition

## Introduction to Programming

### Example Exam Question:

- How to implement encryption and decryption algorithm
- Design a tax calculator (paper will provide a table of income)

### Programs

- Programs can be compiled by using a compiler into machine code (Java, C)
- Programs can also be executed directly from the source code by using an interpreter (e.g. Python, Javascript)

### Library

- Packaged collection of behaviours or capabilities that can be called (or invoked) by a program

### Programming Languages

```
Higher level = close to how humans express themselves
| 4GL Language
| High Level Language
| Low Level Language
| Assembler Language
| Machine Language
v
Lower level = closer to the technical implementation of the computer
```

### Procedural Programming

- An ordered set of steps to solve a problem
- Made of 3 building blocks: Sequencing, Selection, and Iteration
- Good algorithms should be:
  - Unambiguous
  - Defined input
  - Defined set of output
  - Guaranteed to terminate
  - Guaranteed to produce a correct result

### Bubble Sort

```
-> Steps through the list to be sorted
-> Compares each adjacent items
-> Swaps if in wrong order
-> Repeat until no swaps are needed

- Begin with 1st element
- Look at element on the right
- If element should come before the element on the left, swap so that they are in order
- Compare the next element and repeat previous step, repeat until end of array
- Repeat process for n-1 passes when n is the number of elements in the array

E.g.
3 - 4 - 2 - 1 - 5
3 - 2 - 1 - 4 - 5
2 - 1 - 3 - 4 - 5
1 - 2 - 3 - 4 - 5
```

### Java

LTS

- Stands for Long Term Service

Java Standard Edition
Open JDK - Opensource
Oracle JDK - Partially free, but not free for commercial

JDK vs JRE

- JRE: Java Runtime Environment. Includes a Java Virtual Machine (JVM) and core libraries ( The Java API)
- JDK: Java Development Kit.

_Useful Java Packages_

- java.io
- java.lang
- java.net
- java.sql
- java.text
- java.util

_Java Packaging - JAR files_
JAR files are similar to ZIP files

Question:

- Is it safe to say the big O notation for the bubble sort is `O(n)=n-1`?
- What's the JDK that we're using for this course? Using LTS17 (Look for the latest LTS)
