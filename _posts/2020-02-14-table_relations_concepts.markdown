---
layout: post
title:      "Table Relations Concepts"
date:       2020-02-14 17:59:17 -0500
permalink:  table_relations_concepts
---


Data in the backend of most programs that require lots of storage is stored tables, and these tables are created in Structured Query Languge, or SQL (pronounced 'see-qual').  If you want to be able to access the data from the front end, these tables have to be related to one another somehow so the user can search for something as specifically as possible, with as many relevant results from the query as possible.  The data has to have a way to communicate to the methods and objects of the mid or front end program - this is where ORM comes in.  

The first concept that should be considered is the arrangement of all data in a heirarchy.  The most general level of data is a schema.  This holds every piece of data that could be conceivably related.  Below the schema, you can have multiple databases.  Each database holds a number of tables, and each table holds a number of rows.  The tables will relate to each other within the same database but not to other tables within other databases.  

The second piece of information is how these tables relate to each other.  The most common way or relating tables involves access the main key of rows in a table from another table.  This takes the entire piece of data, a row, and relates it to another row in another table, or another id from that row.  Because a row usually represents an object in the program, each row can have many relations to other objects, and the row can have many objects relating to it.  This is called a many-to-many relationship although it could be one-to-many relationship or many-to-one relationship.  

The main way this is represented within the SQL schema is through join tables which can hold the ids of all rows in multiple tables.  Each row in the join table also has an id, so that the data from each row can be selected with a single query.  There are many types of joins and they relate to which data is being selected from which table.  Outer joins exclude certain information, while the opposite is true for Inner joins.  Without specifying, SQL will select data that the two tables have in common.  

When selecting multiple rows of related tables through a query, the user often has input as to which data should be shown.  This is where user input comes in.  Methods and variables can also define information that is queried with use of question marks to represent data.


