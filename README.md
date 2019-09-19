<u> #Database Cheat Sheet# <u>


## This File Will Include All SQL Commands ##

##Types of Databases ##

<u> Relational Database <u>
A set of formally described tables from which data can be accessed or reassembled in many different ways without having to reorganize the database tables.

<u> NoSQL Database <u<>
NoSQL is an approach to database design that can accommodate a wide variety of data models. NoSQL, which stand for "not only SQL," is an alternative to traditional relational databases in which data is placed in tables and data schema is carefully designed before the database is built. NoSQL databases are especially useful for working with large sets of distributed data.


## SQL INFORMATION ##

The standard user and application programming interface (API) of a relational database is the Structured Query Language (SQL).

### Basic SQL Syntax ###

"SELECT * FROM tableName" - The standard SELECT statement
"WHERE" - The keyword that restricts our select query result set and "condition" - The filter to be applied on the results. The filter could be a range, single value or sub query.

USE - use that paricular database
CREATE TABLE name1 - Creates a table called name1
INSERT INTO name1 - Puts data into table called name1
ALTER TABLE name1
alter column Email -  alters Email column in name one

DELETE FROM name1 - Will delete the whole table name1

DELETE FROM name1
WHERE trainer_name = Frank - Will Delete rows where trainer name is Frank

## Data Types ##

- CHAR
- VARCHAR
- BINARY
- BOOL
- FLOAT
- DECIMAL
- DATE

## Arithmetic Operators ##

+ - Add
- - Subtract
* - Multiply
/ - Divide
% - Percentage(Modulo)
< - Less than
> - More than
<= - Less than or equal to
>= More than or equal to



### Normal Form ###

1st Normal Form(1NF)

Make everything atomic( As small as possible)
There shoul be no repeating groups

2nd Normal Form(2NF)

Must always follow first rule (1NF)
All non-key attributes are fully functional depending on the primary key

3rd Normal Form(3NF)

It's in 2NF
There is no transitive functional dependency
- When a non key column is functionally dependant on another non-key column.
Which is functionally dependant on


### Wildcards ###

Can be used as a subsitute for any other characters in a string when using the LIKE operator

& - Substitute fir 0 or more characters
_ - Substitute for single character
[charlist] - Sets and ranges for characters to match [ABC]% - Will bring backi anythingn starting with those letters
[^charlist] - Sets a range of characters that don't match [^ABC]% Will bring back anything that does not start with those letters

IN (ch, hp) - list of things

LIKE 'ch%' - has this word inside word

### Join ###

INNER JOIN(simple join)]
-
LEFT JOIN or OUTER LEFT JOIN

RIGHT JOIN or RIGHT OUTER JOIN

FULL JOIN or FULL OUTER JOIN

SELECT OrderOD, Convert(VARCHAR(10), OrderDate, 103) as [dd/mm/yyy]

### Sub Query ###




Scalar Subquery
A subquery that returns at most one row and one column.

Table Subquery
(with one column)
A subquery that may return any number of rows within one column. A table subquery may only appear on the right hand side of a quantified comparison predicate. This type of predicate compares a single row value of a table to potentially multiple result row values from a subquery.

PointBase supports table subqueries only in a quantified comparison predicate that uses the quantified operators, IN, NOT IN, EXISTS, or NOT EXISTS. Also see "Predicates" for more information about these quantified operators.

Non-correlated Subquery
A subquery that does not use a correlated (outer) reference. It references a column, which an enclosing (outer) query block does not define.

Correlated Subquery
A subquery that uses a correlated reference, sometimes referred to as an "outer reference". It references a column, which an enclosing (outer) query block defines.

Nested Subqueries
A subquery located within another subquery. PointBase supports any level of nested subqueries.


### DDL (Data Definition Language) ###

A data definition language (DDL) is a computer language used to create and modify the structure of database objects in a database. These database objects include views, schemas, tables, indexes, etc.

### DQL (Data Query Language) ###

The SQL commands used to retrieve the data from database is known as Data Query Language (DQL

### DML (Data Manipulation Language) ###

A data manipulation language (DML) is a family of computer languages including commands permitting users to manipulate data in a database. This manipulation involves inserting data into database tables, retrieving existing data, deleting data from existing tables and modifying existing data. DML is mostly incorporated in SQL databases.
