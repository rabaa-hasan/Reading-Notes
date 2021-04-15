# DB Normalization
Database Normalization is a process used to organize databases into tables and columns. The main idea with this is a table should be a specific topic and only supporting topics included. We use a spreadsheet to contain the the information as an example, we can contain data about salespeople and customers.

## There are a few reasons we would want to go through this process:

* Make the database more efficient
* Prevent the same data from being stored in more than one place (called an “insert anomaly”)
* Prevent updates being made to some data but not others (called an “update anomaly”)
* Prevent data not being deleted when it is supposed to be, or from data being lost when it is not supposed to be (called a “delete anomaly”)
* Ensure the data is accurate
* Reduce the storage space that a database takes up
* Ensure the queries on a database run as fast as possible

Normalization in a DBMS is done to achieve these points. Without normalization on a database, the data can be __slow, incorrect,__ and __messy__.

## DB example:

![d](https://www.plus2net.com/sql_tutorial/images/table.jpg)

## Types of Anomalies
### Insertion Anomaly
The insertion anomaly occurs when new record is inserted in relation. In this anomaly user cannot insert a fact about an entity until he has an additional fact about another entity.

### Deletion Anomaly
The deletion anomaly occurs when a record is deleted from the relation. In this anomaly, the deletion of facts about an entity automatically deletes the fact of another entity.

### Modification Anomaly
The modification anomaly occurs when the record is updated in the relation. In this anomaly, the modification in the value of specific attribute requires modification in all records in which that value occurs.

## What is partial dependency? How does partial dependency affect a relation?
### Partial dependency
A type of dependency in which one or more non-key attributes are functionally dependent on a part of primary key is called partial dependency.

## Definition of Database Normalization
There are three common forms of database normalization: 1st, 2nd, and 3rd normal form. They can be abbreviated as 1NF, 2NF, and 3NF.


1. First Normal Form: The information is stored in a relational table with each column containing atomic values.
2. Second Normal Form: The table is in first normal form and all the columns depend on the table's primary key.
3. Third Normal Form: The table is in second normal form and all of its columns are not transitively dependent on the primary key.


