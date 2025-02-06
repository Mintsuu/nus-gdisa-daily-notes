# Fundamentals of Programming with Java

For exams, assume all classes and methods are `public`, assume all methods have the `void` return type.

## Java Modules

- `module-info.java` use if your project is modular (e.g. if designing a calculator, with multiple functions, use this)

## Java Classes

- Class is a template for an object

## System.out.printF()
- Formatting string types:
    - `%d`, `%xd`: integer printed in `x` spaces. If `x` is omitted, spaces = length of integer
    - `%s`, `%xs`: string printed in `x` spaces. Same as above
    - `%f`, `%x.yf, %.yf`: Floating number (float or double), printed in `x` spaces. Same as above. Total width includes all characters in formatted output. 
    - `%n`: System-specific new line
    - `%%`: Percent sign

## DecimalFormat Class
- Used to format decimal numbers using a pattern string
- `#`: Specify the decimal points. E.g. if given `51.424`, using a pattern like `#.##`, the output will be `51.42`. Value will round up to the nearest degree based on the format. If the given number's significant digits exceeds the format, it will just use the most relevant digit. 
- `0`: Same as above, except if the given number exceeds the format, it will insert `0` to the missing significant points.
- `.`: Specify the location of the decimal separator
- `,`: To group numbers together (e.g. #,###.## = 1,495.23)

## Reading Inputs from CLI
- The `Scanner` class is used to get user input (from the `java.util` package
```
import java.utils.Scanner;

Scanner scanner = new Scanner(System.in);
String name = scanner.nextLine();
int age = scanner.nextInt();
double salary = scanner.nextDouble();
scanner.close();
```

Scanner Types:
- `nextBoolean()`
- `nextByte()`
- `nextDouble()`
- etc.

- If there is a mismatch, an `InputMissingException` error will be thrown

## Questions
- What is a static field?

## Potential Exam Questions
- Hotel Booking system, print out the number of rooms in a specific format

