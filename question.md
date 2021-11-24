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


#7. What is a Primary key?
- `Table - SQL Interview Questions - EdurekaA Primary key in SQL is a column (or collection of columns) or a set of columns that uniquely identifies each row in the table.`
- `Uniquely identifies a single row in the table`
- `Null values not allowed`
**Example- In the Student table, Stu_ID is the primary key.**













