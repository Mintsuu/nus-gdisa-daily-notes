## Many-to-many relationship mapping in JPA
- If there are no other attributes in the many-to-many table, can use JPA's setup to create a symbolic link between the 2 entities 
- The other alternate way is to just create the joined foreign keys table as a new entity 
- If there are other attributes/properties in the joined foreign keys table, don't use JPA's setup 

1. SELECT s FROM student s ORDER BY s.matricNo 
2. SELECT s FROM student s WHERE s.name LIKE 'B%'

1. SELECT s from students s JOIN department d ON s.department_id = d.id WHERE s.name LIKE '%man%'

1. SELECT c FROM course c JOIN c.students s WHERE s.matricNo = :searchQuery 
2. SELECT c FROM student s JOIN s.courses c WHERE s.matricNo = :searchQuery

## Questions 
- We learnt in the SQL class that we can create `views` from tables. How do we query that? Do we need to create an entity for it?
