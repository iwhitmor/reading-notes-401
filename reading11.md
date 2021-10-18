# Introduction to Databases and ERDs

## [Data Models (review the DB schema](https://docs.microsoft.com/en-us/aspnet/core/data/ef-mvc/complex-data-model?view=aspnetcore-2.0)

## [DBMS Data Base Management System](https://www.tutorialspoint.com/dbms/dbms_overview.htm)

### Additional Research

* What is a Schema?

  * A DB schema is an abstract design that represents the storage of data in a DB

* Why do we use them?

  * Helps devs visualize how a database should be structured and give clear point of reference about what project contains

* What do they look like?

  * DB schema will include:

    * All important or relevant dats

    * Consisten formatting for all data entries

    * Unique keys for all entries and database objects

    * Each column in a table has a name and data type

* What are the different types of Database Keys?

  * Primary

  * Candidate

  * Super

  * Alternate

  * Composite or Compound

  * Unique

  * Foreign

* What is a Primary Key?

  * The most important key in the DB. There can only be one primary key. The primary key contains unique values

* What is a Foreign Key?

  * A foreign key can be a common key. Using a foreign key we can identify records from multiple tables. It accepts duplicate values as well as null values 

* What is a Composite Key?

  * The composite key can be a combo of primary and candidate keys 

* What are Relationships in a relational database?

  * A situation that exists between two relational database tables when one table has a foreign key that reference the primary key of the other table

* What is a 1:1 relationship?

  * A 1:1 relationship is a link between the information in two tables, where each record in each table only appears once

* What is a Many:Many relationship?

  * A many-to-many relationship refers to a relationship between tables in a database when a parent row in one table contains several child rows in the second table, and vice versa.

* How about a 1: Many?

  * In a relational database, a one-to-many relationship exists when one row in table A may be linked with many rows in table B, but one row in table B is linked to only one row in table A. It is important to note that a one-to-many relationship is not a property of the data, but rather of the relationship itself

#### Additional Resources

* Information taken from the links below:

  * [https://careerkarma.com/blog/database-schema/#:~:text=Database%20schemas%20are%20important%20because,and%20fields%20a%20project%20contains](https://careerkarma.com/blog/database-schema/#:~:text=Database%20schemas%20are%20important%20because,and%20fields%20a%20project%20contains)

  * [https://www.analyticsvidhya.com/blog/2020/07/difference-between-sql-keys-primary-key-super-key-candidate-key-foreign-key/](https://www.analyticsvidhya.com/blog/2020/07/difference-between-sql-keys-primary-key-super-key-candidate-key-foreign-key/)
  
  * [https://www.csestack.org/different-types-database-keys-example/#primary-key](https://www.csestack.org/different-types-database-keys-example/#primary-key)
  
  * [https://support.microsoft.com/en-us/office/video-create-one-to-one-relationships-a5868c76-50ea-44b7-892d-43f2af2802e0](https://support.microsoft.com/en-us/office/video-create-one-to-one-relationships-a5868c76-50ea-44b7-892d-43f2af2802e0)

  * [https://www.techopedia.com/definition/27291/many-to-many-relationship#:~:text=A%20many%2Dto%2Dmany%20relationship%20refers%20to%20a%20relationship%20between,are%20often%20tricky%20to%20represent](https://www.techopedia.com/definition/27291/many-to-many-relationship#:~:text=A%20many%2Dto%2Dmany%20relationship%20refers%20to%20a%20relationship%20between,are%20often%20tricky%20to%20represent)

  * [https://en.wikipedia.org/wiki/One-to-many_(data_model)#:~:text=In%20a%20relational%20database%2C%20a,rather%20of%20the%20relationship%20itself](https://en.wikipedia.org/wiki/One-to-many_(data_model)#:~:text=In%20a%20relational%20database%2C%20a,rather%20of%20the%20relationship%20itself)