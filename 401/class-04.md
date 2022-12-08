[Home](../README.md)

# Class 4

## NoSQL vs SQL

- SQL is better suited for the complex query environment.
- NoSQL is better for representing hierarchical data with deep nesting.
- SQL databases scale vertically by requiring more resources on the machine, whereas NoSQL databases scale horizontally by adding more machines.
- In SQL, keywords are capitalized by convention, and parameters are generally lowercase
- Normalization refers to removing duplicate data in db consisting of a set of related tables.

## SQL Modeling Techniques

- A one-to-many relation is where a field in a SQL table points to multiple records in another table. For example, a customer record might have an orders field that is an array of order IDs pointing to all of their past orders in the orders table.
- Conversely, the orders table may share a many-to-one relationship with the customers table where many different orders have a customers field pointing to the same customer
- A one-to-one relationship means a single record in one table is uniquely and exclusively related to another single record in a different table
- It is useful to create a diagram of a SQL database to model its structure and relations prior to creating it.
- A primary key is one that can uniquely identify a single record in a table.
