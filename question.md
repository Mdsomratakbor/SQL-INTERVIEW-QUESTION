# 1. What is the difference between SQL and MySQL?
<table border="1"><caption><p style="text-align: center;"><strong><span> SQL vs MySQL</span></strong></p></caption><tbody><tr style="height: 41.1563px;"><td><span><strong>SQL</strong></span></td><td><span><strong>MySQL</strong></span></td></tr><tr style="height: 48px;"><td style="padding: 5px; width: 394px; text-align: justify; height: 48px;"><span>SQL is a standard language which stands for Structured Query Language based on the English language<a name="subsetsofsql"></a> </span></td><td style="padding: 5px; width: 365px; text-align: justify; height: 48px;"><span>MySQL is a database management system. </span></td></tr><tr><td style="padding: 5px; width: 394px; text-align: justify;"><span>SQL is the core of the relational database which is used for accessing and managing database</span></td><td style="padding: 5px; width: 365px; text-align: justify;"><p style="text-align: justify;"><span>MySQL is an RDMS (Relational Database Management System) such as SQL Server, Informix etc.</span></p></td></tr></tbody></table>

# 2. What are the different subsets of SQL?
- Data Definition Language (DDL) – It allows you to perform various operations on the database such as CREATE, ALTER, and DELETE objects.
- Data Manipulation Language(DML) – It allows you to access and manipulate data. It helps you to insert, update, delete and retrieve data from the database.
- Data Control Language(DCL) – It allows you to control access to the database. Example – Grant, Revoke access permissions.

# 3. What do you mean by DBMS? What are its different types?
`Database - SQL Interview Questions - EdurekaA Database Management System (DBMS) is a  software application that interacts with the user, applications, and the database itself to capture and analyze data. A database is a structured collection of data. `

`A DBMS allows a user to interact with the database. The data stored in the database can be modified, retrieved and deleted and can be of any type like strings, numbers, images, etc.`

**There are two types of DBMS:**

- Relational Database Management System: The data is stored in relations (tables). Example – MySQL.
- Non-Relational Database Management System: There is no concept of relations, tuples and attributes.  Example – MongoDB


# 4. What do you mean by table and field in SQL?
`A table refers to a collection of data in an organised manner in form of rows and columns. A field refers to the number of columns in a table.`
**For example:**

`Table: StudentInformation`
`Field: Stu Id, Stu Name, Stu Marks`

# 5. What are joins in SQL?
`A JOIN clause is used to combine rows from two or more tables, based on a related column between them. It is used to merge two tables or retrieve data from there. There are 4 types of joins, as you can refer to below:`

- **Inner join:** `Inner Join in SQL is the most common type of join. It is used to return all the rows from multiple tables where the join condition is satisfied.`
- **Left Join:**  `Left Join in SQL is used to return all the rows from the left table but only the matching rows from the right table where the join condition is fulfilled.`
- **Right Join:** `Right Join in SQL is used to return all the rows from the right table but only the matching rows from the left table where the join condition is fulfilled.`
- **Full Join:** `Full join returns all the records when there is a match in any of the tables. Therefore, it returns all the rows from the left-hand side table and all the rows from the right-hand side tablen`


# 6. What is the difference between CHAR and VARCHAR2 datatype in SQL?
`Both Char and Varchar2 are used for characters datatype but varchar2 is used for character strings of variable length whereas Char is used for strings of fixed length. For example, char(10) can only store 10 characters and will not be able to store a string of any other length whereas varchar2(10) can store any length i.e 6,8,2 in this variable.`


# 7. What is a Primary key?
- `Table - SQL Interview Questions - EdurekaA Primary key in SQL is a column (or collection of columns) or a set of columns that uniquely identifies each row in the table.`
- `Uniquely identifies a single row in the table`
- `Null values not allowed`
**Example- In the Student table, Stu_ID is the primary key.**

# 8. What are Constraints?
Constraints in SQL are used to specify the limit on the data type of the table. It can be specified while creating or altering the table statement. The sample of constraints are:
- NOT NULL
- CHECK
- DEFAULT
- UNIQUE
- PRIMARY KEY
- FOREIGN KEY


# 9. What is the difference between DELETE and TRUNCATE statements?
<table style="height: 158px;" border="1" width="100%"><caption><p style="text-align: center;"><strong><span> DELETE vs TRUNCATE</span></strong></p></caption><tbody><tr style="height: 41.1563px;"><td><span><strong>DELETE</strong></span></td><td><span><strong>TRUNCATE</strong></span></td></tr><tr style="height: 48px;"><td style="padding: 5px; width: 394px; text-align: justify; height: 48px;"><span>Delete command is used to delete a row in a table.</span></td><td style="padding: 5px; width: 365px; text-align: justify; height: 48px;"><span>Truncate is used to delete all the rows from a table.</span></td></tr><tr style="height: 24px;"><td style="padding: 5px; width: 394px; text-align: justify; height: 24px;"><span>You can rollback data after using delete statement.<a name="uniquekey"></a></span></td><td style="padding: 5px; width: 365px; text-align: justify; height: 24px;"><span>You cannot rollback data.</span></td></tr><tr style="height: 24px;"><td style="padding: 5px; width: 394px; text-align: justify; height: 24px;"><span>It is a DML command.</span></td><td style="padding: 5px; width: 365px; text-align: justify; height: 24px;"><span>It is a DDL command.</span></td></tr><tr style="height: 24px;"><td style="padding: 5px; width: 394px; text-align: justify; height: 24px;"><span>It is slower than truncate statement.</span></td><td style="padding: 5px; width: 365px; text-align: justify; height: 24px;"><span>It is faster.</span></td></tr></tbody></table>


# 10. What is a Unique key?
- Uniquely identifies a single row in the table.
- Multiple values allowed per table.
- Null values allowed. 

# 11. What is a Foreign key in SQL?
- Foreign key maintains referential integrity by enforcing a link between the data in two tables.
- The foreign key in the child table references the primary key in the parent table.
- The foreign key constraint prevents actions that would destroy links between the child and parent tables.

# 12. What do you mean by data integrity? 
`Data Integrity defines the accuracy as well as the consistency of the data stored in a database. It also defines integrity constraints to enforce business rules on the data when it is entered into an application or a database.`

# 13. What is the difference between clustered and non-clustered index in SQL?
The differences between the clustered and non clustered index in SQL are :

- `Clustered index is used for easy retrieval of data from the database and its faster whereas reading from non clustered index is relatively slower.`
- `Clustered index alters the way records are stored in a database as it sorts out rows by the column which is set to be clustered index whereas in a non clustered index, it does not alter the way it was stored but it creates a separate object within a table which points back to the original table rows after searching.`
- `One table can only have one clustered index whereas it can have many non clustered index.`

# 14. What do you understand by query optimization?
`The phase that identifies a plan for evaluation query which has the least estimated cost is known as query optimization.`
`The advantages of query optimization are as follows:`
- `The output is provided faster`
- `A larger number of queries can be executed in less time`
- `Reduces time and space complexity`

# 15. What do you mean by Denormalization?
`Denormalization refers to a technique which is used to access data from higher to lower forms of a database. It helps the database managers to increase the performance of the entire infrastructure as it introduces redundancy into a table. It adds the redundant data into a table by incorporating database queries that combine data from various tables into a single table.`

# 16. What is an Index?
`An index refers to a performance tuning method of allowing faster retrieval of records from the table. An index creates an entry for each value and hence it will be faster to retrieve data.`

# 17. Explain different types of index in SQL.
`There are three types of index in SQL namely:`

**Unique Index:**
`This index does not allow the field to have duplicate values if the column is unique indexed. If a primary key is defined, a unique index can be applied automatically.`

**Clustered Index:**
`This index reorders the physical order of the table and searches based on the basis of key values. Each table can only have one clustered index.`

**Non-Clustered Index:**
`Non-Clustered Index does not alter the physical order of the table and maintains a logical order of the data. Each table can have many nonclustered indexes.`

# 18. What is Normalization and what are the advantages of it?
`Normalization in SQL is the process of organizing data to avoid duplication and redundancy. Some of the advantages are:`

- `Better Database organization`
- `More Tables with smaller rows`
- `Efficient data access`
- `Greater Flexibility for Queries`
- `Quickly find the information`
- `Easier to implement Security`
- `Allows easy modification`
- `Reduction of redundant and duplicate data`
- `More Compact Database`
- `Ensure Consistent data after modification`

# 19. Explain different types of Normalization.
`There are many successive levels of normalization. These are called normal forms. Each consecutive normal form depends on the previous one.The first three normal forms are usually adequate.`

- **First Normal Form (1NF)** – `No repeating groups within rows`
- **Second Normal Form (2NF)** – `Every non-key (supporting) column value is dependent on the whole primary key.`
- **Third Normal Form (3NF)** – `Dependent solely on the primary key and no other non-key (supporting) column value.`

# 20. What is the ACID property in a database?
`ACID stands for Atomicity, Consistency, Isolation, Durability. It is used to ensure that the data transactions are processed reliably in a database system.` 

**Atomicity:** `Atomicity refers to the transactions that are completely done or failed where transaction refers to a single logical operation of a data. It means if one part of any transaction fails, the entire transaction fails and the database state is left unchanged.`
**Consistency:** `Consistency ensures that the data must meet all the validation rules. In simple words,  you can say that your transaction never leaves the database without completing its state.`
**Isolation:** `The main goal of isolation is concurrency control.`
**Durability:** `Durability means that if a transaction has been committed, it will occur whatever may come in between such as power loss, crash or any sort of error.`


# 21. What do you mean by “Trigger” in SQL?
`Trigger in SQL is are a special type of stored procedures that are defined to execute automatically in place or after data modifications. It allows you to execute a batch of code when an insert, update or any other query is executed against a specific table.`

# 22. What are the different operators available in SQL?
`There are three operators available in SQL, namely:`

- `Arithmetic Operators`
- `Logical Operators`
- `Comparison Operators`


# 23. Are NULL values same as that of zero or a blank space? 
`A NULL value is not at all same as that of zero or a blank space. NULL value represents a value which is unavailable, unknown, assigned or not applicable whereas a zero is a number and blank space is a character.`

# 24. What is the difference between cross join and natural join?
`The cross join produces the cross product or Cartesian product of two tables whereas the natural join is based on all the columns having the same name and data types in both the tables.`

# 25. What is subquery in SQL?
`A subquery is a query inside another query where a query is defined to retrieve data or information back from the database. In a subquery, the outer query is called as the main query whereas the inner query is called subquery. Subqueries are always executed first and the result of the subquery is passed on to the main query. It can be nested inside a SELECT, UPDATE or any other query. A subquery can also use any comparison operators such as >,< or =.`

# 26. What are the different types of a subquery?
`There are two types of subquery namely, Correlated and Non-Correlated.`

**Correlated subquery:** `These are queries which select the data from a table referenced in the outer query. It is not considered as an independent query as it refers to another table and refers the column in a table.`

**Non-Correlated subquery:** `This query is an independent query where the output of subquery is substituted in the main query.`

# 27. What is the need for group functions in SQL? 
`Group functions work on the set of rows and return one result per group. Some of the commonly used group functions are`: **AVG, COUNT, MAX, MIN, SUM, VARIANCE.**

# 28. What is a Relationship and what are they?
`Relation or links are between entities that have something to do with each other. Relationships are defined as the connection between the tables in a database. There are various relationships, namely:`

- `One to One Relationship.`
- `One to Many Relationship.`
- `Many to One Relationship.`
- `Self-Referencing Relationship.`


# 29. How can you insert NULL values in a column while inserting the data?
`NULL values in SQL can be inserted in the following ways:`

- Implicitly by omitting column from column list.
- Explicitly by specifying NULL keyword in the VALUES clause

# 30. What is the main difference between ‘BETWEEN’ and ‘IN’ condition operators?
`BETWEEN operator is used to display rows based on a range of values in a row whereas the IN condition operator is used to check for values contained in a specific set of values.`

`Example of BETWEEN:`
**SELECT * FROM Students where ROLL_NO BETWEEN 10 AND 50;**
`Example of IN:`
**SELECT * FROM students where ROLL_NO IN (8,15,25);**

# 31. Why are SQL functions used?
`SQL functions are used for the following purposes:`

- `To perform some calculations on the data`
- `To modify individual data items`
- `To manipulate the output`
- `To format dates and numbers`
- `To convert the data types`

# 32. What is the need for MERGE statement?
`This statement allows conditional update or insertion of data into a table. It performs an UPDATE if a row exists, or an INSERT if the row does not exist.`

# 33. What do you mean by recursive stored procedure?
`Recursive stored procedure refers to a stored procedure which calls by itself until it reaches some boundary condition. This recursive function or procedure helps the programmers to use the same set of code n number of times.`

# 34. What is CLAUSE in SQL?
`SQL clause helps to limit the result set by providing a condition to the query. A clause helps to filter the rows from the entire set of records.`

`For example` – **WHERE, HAVING clause.**

# 35. What is the difference between ‘HAVING’ CLAUSE and a ‘WHERE’ CLAUSE?
`HAVING clause can be used only with SELECT statement. It is usually used in a GROUP BY clause and whenever GROUP BY is not used, HAVING behaves like a WHERE clause.`
`Having Clause is only used with the GROUP BY function in a query whereas WHERE Clause is applied to each row before they are a part of the GROUP BY function in a query.`

# 36. List the ways in which  Dynamic SQL can be executed?
`Following are the ways in which dynamic SQL can be executed:`

- Write a query with parameters.
- Using EXEC.
- Using sp_executesql.
# 37. What are the various levels of constraints?
`Constraints are the representation of a column to enforce data entity and consistency. There are two levels  of a constraint, namely:`

- column level constraint
- table level constraint
# 38. List some case manipulation functions in SQL?
`There are three case manipulation functions in SQL, namely:`

- **LOWER:** `This function returns the string in lowercase. It takes a string as an argument and returns it by converting it into lower case. Syntax:
 LOWER(‘string’)`
- **UPPER:** `This function returns the string in uppercase. It takes a string as an argument and returns it by converting it into uppercase. Syntax:
UPPER(‘string’)`
- **INITCAP:** `This function returns the string with the first letter in uppercase and rest of the letters in lowercase. Syntax:
 INITCAP(‘string’)`
 
 # 39. What are the different set operators available in SQL?
`Some of the available set operators are – Union, Intersect or Minus operators`

# 40. What is an ALIAS command?
`ALIAS command in SQL is the name that can be given to any table or a column. This alias name can be referred in WHERE clause to identify a particular table or a column.`

**For example-** `Select emp.empID, dept.Result from employee emp, department as dept where emp.empID=dept.empID`

# 41. What are aggregate and scalar functions?
`Aggregate functions are used to evaluate mathematical calculation and returns a single value. These calculations are done from the columns in a table. For example- max(),count() are calculated with respect to numeric.`

`Scalar functions return a single value based on the input value. For example – UCASE(), NOW() are calculated with respect to string.`

# 42. Name the operator which is used in the query for pattern matching?
`LIKE operator is used for pattern matching, and it can be used as -.`

`% – It matches zero or more characters.`
`For example- select * from students where studentname like ‘a%’`

`_ (Underscore) – it matches exactly one character.`
`For example- select * from student where studentname like ‘abc_’`

# 43. What is the main difference between SQL and PL/SQL?
`SQL is a query language that allows you to issue a single query or execute a single insert/update/delete whereas PL/SQL is Oracle’s “Procedural Language” SQL, which allows you to write a full program (loops, variables, etc.) to accomplish multiple operations such as selects/inserts/updates/deletes.`

# 44. What is a View?
`A view is a virtual table which consists of a subset of data contained in a table. Since views are not present, it takes less space to store. View can have data of one or more tables combined and it depends on the relationship.`

# 45. What are Views used for?
`A view refers to a logical snapshot based on a table or another view. It is used for the following reasons:`

- Restricting access to data.
- Making complex queries simple.
- Ensuring data independence.
- Providing different views of same data.

# 46. What is a Stored Procedure?
`A Stored Procedure is a function which consists of many SQL statements to access the database system. Several SQL statements are consolidated into a stored procedure and execute them whenever and wherever required which saves time and avoid writing code again and again.`

# 47. List some advantages and disadvantages of Stored Procedure?
**Advantages:**
`A Stored Procedure can be used as a modular programming which means create once, store and call for several times whenever it is required. This supports faster execution. It also reduces network traffic and provides better security to the data.`

**Disadvantage:**
`The only disadvantage of Stored Procedure is that it can be executed only in the database and utilizes more memory in the database server.`

# 48. List all the types of user-defined functions?
`There are three types of user-defined functions, namely:`

- Scalar Functions
- Inline Table-valued functions
- Multi-statement valued functions

# 49. What do you mean by Collation?
`Collation is defined as a set of rules that determine how data can be sorted as well as compared. Character data is sorted using the rules that define the correct character sequence along with options for specifying case-sensitivity, character width etc.`

# 50. What are the different types of Collation Sensitivity?
`Following are the different types of collation sensitivity:`

- Case Sensitivity: A and a and B and b.
- Kana Sensitivity: Japanese Kana characters.
- Width Sensitivity: Single byte character and double-byte character.
- Accent Sensitivity.











