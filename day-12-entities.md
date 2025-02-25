# Entities

## Business Entities 
- Info that is a property of something else 
- E.g. library user is a business entity, sex is a property of the user, so its not a business entity 
- Info is not stored but is created on demand 
- E.g. product inventory may not be a business entity 
- If data can be regenerated with another set of data, then there's no need to store that particular info 

### Types of Use Cases 
- Supporting Business Operations 
  - E.g. providing customers with invoice from last visit using regenerated info
- Supporting DDPP 
- Supporting BackOffice Operations 
  - E.g. need to keep documents for audit

## Domain Models 
- Good brief descriptions describes scope
- Bad one lists the properties (not necessary as this will be done during the database design stage)

## Class Diagram 
- Arrow towards action: Can write 
- Arrow pointing towards user: Can read

## Activity Diagram Feedback
- Base on the perspective of an application
- If the application needs to wait for a period of time, end the activity diagram and start a new one with a separate scheduler program
```
Visa application

List tours that are fully booked/confirmed assigned to the tour leader
|
V
Select a tour 
|
V
List of customers in tour and their citizenship 
|
V
Print PDF of all customers who needs visa
|
V 
O 
```

