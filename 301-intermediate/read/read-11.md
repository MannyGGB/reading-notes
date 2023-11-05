# Reading 11

(https://www.thegeekstuff.com/2014/01/sql-vs-nosql-db/?utm_source=tuicool)

- Fill in the chart below with five differences between SQL and NoSQL databases:

| **SQL**                                                                | **NoSQL**                                                         |
| ---------------------------------------------------------------------- | ----------------------------------------------------------------- | ------------------------------------------------------------------- |
| Relational databases: data is structured and organised.                | Distributed databases: data is added, similar to a list of items. |
| Table based: how data is structured in table rows.                     | Document based: it is a collection of data.                       |
| Predefined schema.                                                     | Dynamic schema.                                                   |
| SQL language (Structured Query language)                               | UnQL: Each database uses its own syntax.                          |
| Support: excellent support from vendors and independent consultations. |                                                                   | Support: community-based support in some cases and limited experts. |

- What kind of data is a good fit for an SQL database? Any kind of structured data.
- Give a real world example. Inventories, financial transactions, customer information.
- What kind of data is a good fit a NoSQL database? Unstructured data without a traditional organisation method.
- Give a real world example. To store large amounts of data, images, social media posts, documents.
- Which type of database is best for hierarchical data storage? NoSQL databases are better for hierarchical data storage because it stores data using the key-value pair, similar to JSON data.
- Which type of database is best for scalability? SQL databases scale vertically, meaning that increasing the hardware power in one server is enough to handle more data load. NoSQL databases scale horizontally, so you need to add more servers to handle the data load. I would say NoSQL databases are better for scalability because they don't rely on a single server and were programmed with scalability in mind.

(https://www.youtube.com/watch?v=ZS_kXvOeQ5Y)

- What does SQL stand for? Structured Query Language. We use SQL to write database queries with keywords, such as SELECT and FROM.
- What is a relational database? It is a database that works with a predefined, strict structure. We can create relations between the data in different containers or tables.
- What type of structure does a relational database work with? For SQL databases, we use tables with fields (columns) and records (rows).
- What is a ‘schema’? It is the structure we use to organise the data. It is how we organise the data in our data container. We can define the schema using fields (the headings for the table).
- What is a NoSQL database? It is a database which seals with a large number of data in a unstructred way.
- How does it work? You can store data without a predefined schema flexibly in one place. You can always add more data to the database without having to worry about following a schema.
- What is inside of a MongoDB database? A database has a number of collections with documents inside, which can have different schema. The data looks similar to JSON syntax.
- Which is more flexible - SQL or MongoDB? and why. You could argue NoSQL is more flexible because you can change the schema as you go, but SQL is better at consistency with a fixed schema (you know that if a field is empty, there is no record for it). In the end, it depends on the app we are designing and the data we want to store. Usually companies use both types of databases to store different kinds of data.
- What is the disadvantage of a NoSQL database? You can have duplicated data in different collections, so if the data changes, you have to update all the documents with the new data.
- Notes: SQL is usually better for data that changes often because it is easy to update, whereas NoSQL is better at reading large amounts of data. Scaling is also important because SQLs scale vertically (CPUs/hardware) and there is always a power limit, and NoSQLs scale horizontally (servers/software).
