# SQL Statements
## Self-join
- Duplicate the exact same table into different aliases and query each of them with the respective attributes

## Group By
- Essentially functions the same as `DISTINCT`
- Lists down the unique attributes of the given column 

## Group By with Count 
- The `GROUP BY` syntax will automatically group the rows together based on the parameter, so the `COUNT` syntax will count all the necessary rows (To experiment with this for better understanding)

## Group By and Having 
- `HAVING` essentially applies a condition necessary for an attribute to have 

## Union 
- Combine tables with the same columns together (the tables are joined as additional rows)

## Limit 
- Limits the number of rows that can be returned in the output 

## Inner Joins 
- Multiple ways to perform an inner join, no need to always use the `INNER JOIN` syntax 
- Can use `WHERE` and just match the primary key of the parent table to the foreign key of the child table
 

## Sub-queries vs Joins 
- Sub-queries usually used during comparisons
- If information is just from 2 tables, use sub-query
- When combining more than 2 tables, use a join 
- If you're doing a comparison, use a sub-query 
```
e.g. 
SELECT MovieTitle, RentalPrice 
FROM Movies 
WHERE RentalPrice > (SELECT AVG(RentalPrice) FROM Movies)
```

# Data Manipulation Language 
- Exams won't test anything related to DML (`INSERT`, `DELETE`, `UPDATE`)

# Database Definition Language 
##  Commands 
- `CREATE`: Creating tables
- `DROP`: Deleting tables
- `ALTER`: Updating table properties 

## Index
- An index will speed up selection on search keys 

## Constraints 
- `DELETE CASCASE`: Rows that are deleted on the child table will also delete linked rows from the parent table 

# User Views 
- Functions as any other table, but you limit the columns that the view is only allowed to see 
- Keys and integrity constraints cannot be specifically set for user views 

```
CREATE VIEW view-name 
(column names, ...)
AS query
```

# Store Procedures
- Execute SQL statements like a function (can also declare function parameters by specifying the parameter types e.g. INTEGER or CHAR(50))

```
CREATE PROCEDURE procedure_name
AS 
BEGIN 
  --SQL Statements--
END
```

## User Views 
- Mainly used to set permissions, but might be a good way to setup abstract data structures for web application components for web developers to access the information that only they need to know 
- Doesn't seem to have any performance benefits or demerits, just an abstraction layer to limit the kind of information that can be accessed 

## Exams 
- May ask to create tables
- May ask to create constraints 
- Ensure each of the properties are set correctly (e.g. NOT NULL)
- Stored procedures may be tested in exams 
- For stored procedures, add the `AS` in a new line 

## Questions
- Is it safe to say that `GROUP BY` allows you to find distinct values of a certain column vs `DISTINCT` which only finds the distinct rows? 
- Are views used to save computation time from querying multiple tables (assume that you create a view that will mainly be accessed often)?
- Are views just a middleware to inject certain permissions restrictions in SQL queries?

