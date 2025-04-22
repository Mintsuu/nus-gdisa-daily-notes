## Importance of Foreign Keys 
- To promote referential integrity 

## Data Broker 

## Creating Views in place of tables 
- Views basically abstractifies the SQL statements 
- Doesn't provide any performance benefits (whatever SQL statements that's conducted in the creation of the view, it will still be executed)
- Also not able to create constraints 

## Exam Notes 
- If you wanna define an abstract class in exams, ensure that you put <<abstract>> in the class diagram

@startuml

class "ShoppingCart" as shoppingCart {
__
+computeTotal()
}

entity "Product" as product {
-price
-appliedDiscount
__
+getDiscountedPrice()
+getProductType()
}

entity "Flower" as flower {
-valentineDayPromotion
-colour
__
+getColour()
}

entity "Toy" as toy {
-childrenDayPromotion
-trademark
__
+getTrademark()
}

product <|-- toy
product <|-- flower
shoppingCart o-- product



@enduml

@startuml
actor Customer as customer
boundary ShoppingCart as shoppingCart
entity Product as product

customer -> shoppingCart : 1. computeTotal()
activate shoppingCart
shoppingCart -> product : 2. getAppliedDiscount()
activate product
product -> product : 3. getProductType()
product -> product : 4. getDiscountedPrice()
product -> shoppingCart : 5. showDiscountedPrice()
deactivate product
deactivate shoppingCart
@enduml



@startuml

title Scenario 2

interface "PaymentMethod \n <<interface>>" as paymentMethod {
__
+processPayment()
}

class "CreditCard" as creditCard {
-cardNo
-expiryDate
__
+validateCard()
+processPayment()
}

class "BankTransfer" as bankTransfer {
-bankName
-accountNo
__
+verifyBank()
+processPayment()
}

note top of paymentMethod : Using an interface since there are no common attributes\n that's relevant for both CreditCard and BankTransfer payment methods

paymentMethod <|.. creditCard
paymentMethod <|.. bankTransfer

newpage

title Scenario 1

abstract class "Employee" as employee {
-name
-employeeId
-department
__
{abstract} calculateSalary() <<abstract>>
getDetails()
}

class "FullTimeEmployee" as fullTimeEmployee {
-bonus
__
calculateSalary()
}

class "ContractEmployee" as contractEmployee {
-hourlyRate
__
calculateSalary()
}

note top of employee : Using a abstract superclass since there are still common attributes\n that's relevant for both FullTimeEmployee and ContractEmployee

employee <|-- fullTimeEmployee
employee <|-- contractEmployee

@enduml


