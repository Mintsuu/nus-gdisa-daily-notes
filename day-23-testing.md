# Software Testing 
## Benefits of early software testing 
- Cost reduction (Faults found later in the life cycle costs 10-100x more to fix) 
- Risk management and aversion technique 
- Process improvement (Preventive-Detective-Corrective cycle)
- Improves product quality 

## Equivalent Classes 
- Identify equivalent classes so you can test:
  - Range of values
  - Type
  - A number of correct values 
  - A set of correct values 
  - Exceptions 

### Range of values 
- E.g. Company only offers a bonus from 10-20%
  - Check if 15% is valid 
  - Check if 10% is valid 
  - Check if 20% is valid 
  - Check if 5% is invalid 
  - Check if 26% is invalid 

### Type of Value 
- E.g. Credit hours must be a positive integer 
  - Check if 1 is valid 
  - Check if -10 is invalid 
  - Check if 10.1 is invalid 
  - Check if "test" is invalid

### A set of correct values 
- Only "Graduate", "Masters", and Professional Diploma students are allowed to borrow this borrow
- Check if student is a graduate diploma student is valid 
- Check if a masters student is valid 
- Check if a short course student is invalid

## Top Down / Bottom Up Testing 
### Top Down Testing
- Start from the biggest use case and go through the sub use cases to test them out 
- Make sure that they're functioning properly before moving on to the lower level programs 

### Bottom Up Testing 
- Start from the lowest level programs and move upwards instead

## Functional Testing 
- Test for each use case to make sure that it performs as intended in the described use case 
- Not exhaustive 
- Covers the business logic in a sense 
- E.g. Tour Selection -> New Booking -> Enquiring Booking --> Confirm Booking 

## Regression Testing 
- To ensure that the new features of the program will not negatively affect the existing system 
- E.g. In a GST calculator, when the GST value changes, it should not affect the other components of the application 


