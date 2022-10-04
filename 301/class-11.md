[Home](../README.md)

# Class 11

## SQL and NoSQL

|SQL|NoSQL|
|---|---|
| relational | document-based, kv store, graph, wide-column store|
| pre-defined schema | dyanamic-schema |
| vertically scalable | horizontally scalable |
| best fit for complex queries | best fit for hierarchechal data |
| ACID properties (Atomicity, Consistency, Isolation and Durability) | CAP properties (Consistency, Availability and Partition tolerance) |

1. What kind of data is a good fit for an SQL database?
  Data with defined relationships and complex queries.

2. Give a real world example.
  Transactional data and requests

3. What kind of data is a good fit for a NoSQL database?
  Hierarchechal data.

4. Give a real world example.
  Big data.

5. Which type of database is best for hierarchical data storage?
  NoSQL

6. Which type of database is best for scalability?
  Both can scale, although SQL databases scale veritcallyby increasing machine performance and resources, while NoSQL scales horizontally by adding more servers.

## SQL vs NoSQL cont'd

1. What does SQL stand for?
  Structured Query Language.

2. What is a relational database?
  A database where different fields and tables have specific relationships with each other. (one-to-one, one-to-many, many-to-many).

3. What type of structure does a relational database work with?
  Relational DBs work with tables.

4. What is a ‘schema’?
  A schema is a predefined format for entries in a database. All entries must adhere to the schema.

5. What is a NoSQL database?
  A NoSQL is non-relational, and entries are not restricted to any specific schema.

6. How does it work?
  It uses collections, with documents within, that are stored as JSON.

7. What is inside of a Mongo database?
  Mongo DB is a document store DB that stores data in the form of JSON.

8. Which is more flexible - SQL or MongoDB? and why.
  MongoDB is more flexible because it is schema-less and allows you to store data however you choose. On the other hand, it does not support frequent writes or updates to data as well as a relational DB.

9. What is the disadvantage of a NoSQL database?
  They do not support as complex queries as a SQL DB. They are not always as stable as SQL DBs.
