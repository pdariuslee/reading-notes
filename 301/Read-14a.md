# DATABASE NORMALIZATION

## [Database Normalization (Explained in Simple English)](https://www.essentialsql.com/get-ready-to-learn-sql-database-normalization-explained-in-simple-english/#)

### From essentialSQL


- Introduction to Database Normalization

  - Database normalization is a process used to organize a database into tables and columns.  The main idea with this is that a table should be about a specific topic and only supporting topics included. Take a spreadsheet containing the information as an example, where the data contains salespeople and customers serving several purposes:

    - Identify salespeople in your organization
    
    - List all customers your company calls upon to sell a product

    - Identify which salespeople call on specific customers.

- Reasons for Database Normalization

  - There are three main reasons to normalize a database.  The first is to minimize duplicate data, the second is to minimize or avoid data modification issues, and the third is to simplify queries. 

- Data Duplication and Modification Anomalies

  - It increases storage and decrease performance.

  - It becomes more difficult to maintain data changes.

- Search and Sort Issues

  - The last reason we’ll consider is making it easier to search and sort your data.  In the SalesStaff table if you want to search for a specific customer such as Ford, you would have to write a query like


--- 


[Back to Home](https://pdariuslee.github.io/reading-notes/)
