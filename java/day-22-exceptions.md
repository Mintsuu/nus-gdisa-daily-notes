# Exceptions
## `finally`
- Always executes, regardless of whether there was a thrown exception or not 
- In the instance where a scanner is used (and must be closed), better to close it in `finally` rather than after the `catch` block, since there are instances where the application ends (e.g. during an uncaught exception) and it never reaches the end of the application. 

## Catering for all exceptions
- Creating a new `Exception` requires you to explicitly indicate which exception is being thrown 
- Base exception class seems to not have any "throwable" calls, therefore the function will need explicit instructions on how to handle the throwing method
```
If `exception` extends Exception:

public void function getNoise() throws MyException

If `exception` extends RuntimeException:

public void function getNoise() 
```

## Exam Notes 
- Any exceptions will be informed in the paper 
- Not allowed to use the catchall `Exception` in exams

