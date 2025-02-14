# String Manipulation & Random

## 2 Different Ways to Generate Random Values
- `Math.random()` and `new Random()`
- Use built in methods for `new Random()` such as `.nextInt()`

## String Quirks
- Is not a primitive type
- Can be implicitly converted into an `integer` or `byte`
- Numerical values can be compared with one another, but it's case sensitive
- Use `.contains()` string method to compare between different strings, else the usual `==` will compare the numerical values
- `.charAt(n)` to select specific index position of a string. Value type is `char`
- Can use `.replace()` to find and replace instances. 
- `Stringbuffer` class allows you to pre-define string lengths for manipulation
- `Stringbuffer` not covered for exams, but can be used for solutions in exams

## Chars
- Only stores 1 character
- Not valid
    - `''`: Needs at least 1 character
    - `'ab'`: Can only store 1 character
- Similar to string, can also be treated as a number
- 

## Exam Question
- Will definitely have a couple of string manipulation questions
- Will have a briefing on exams on Tuesday

## Trivia
- Capital letters have numerically lower values compared to their lowercase counterparts (based on the ASCII table)

