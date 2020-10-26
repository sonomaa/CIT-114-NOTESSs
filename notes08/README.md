# Notes 8: Databases

### __What is a Database__
- A database is a shared collection of related data used to support the activities of a particular organization. A database can be viewed as a repository of data that is defined once and then accessed by various users. 
- A representation of some aspect of the real world or a collection of data elements (facts) representing real-world information.
- A database management system (DBMS) is a collection of programs that enables users to create and maintain databases and control all access to them. The primary goal of a DBMS is to provide an environment that is both convenient and efficient for users to retrieve and store information.

### Characteristics and Benefits of a DB
- Self-describing nature of a database system: self-describing because it not only contains the database itself, but also metadata which defines and describes the data and relationships between tables in the database.
- Insulation between program and data: In the file-based system, the structure of the data files is defined in the application programs so if a user wants to change the structure of a file
- Support for multiple views of data:  A view is a subset of the database, which is defined and dedicated for particular users of the system. Multiple users in the system might have different views of the system. 
- Sharing of data and multiuser system: Current database systems are designed for multiple users. That is, they allow many users to access the same database at the same time
- Control of data redundancy: In the database approach, ideally, each data item is stored in only one place in the database. Redundancy is controlled by application programming and kept to minimum by introducing as little redudancy as possible when designing the database.
- Data sharing: The integration of all the data, for an organization, within a database system has many advantages. First, it allows for data sharing among employees and others who have access to the system. Second, it gives users the ability to generate more information from a given amount of data than would be possible without the integration.
- Enforcement of integrity constraints: constraints to ensure that users enter valid information and maintain data integrity. A database constraint is a restriction or rule that dictates what can be entered or edited in a table. 
- Restriction of unauthorized access: a security subsystem to create and control different types of user accounts and restrict unauthorized access.  one user might have read-only access, while another might have read and write privileges. 
- Data independence: The system data descriptions or data describing data (metadata) are separated from the application programs. 
- Transaction processing: data remains consistent and valid during transaction processing even if several users update the same information.
- Provision for multiple views of data: By its very nature, a DBMS permits many users to have access to its database either individually or simultaneously.
- Backup and recovery facilities: Backup and recovery are methods that allow you to protect your data from loss.  The database system provides a separate process, from that of a network backup, for backing up and recovering data.

### Fundamental Concepts in the Relational Data Model
- Relation: AKA a table or file, is a subset of the Cartesian product of a list of domains characterized by a name. And within a table, each row represents a group of related data values. 
- Table: The principal storage units are called columns or fields or attributes. These house the basic components of data into which your content can be broken down.
- Domain: A domain is the original sets of atomic values used to model data. 
- Records: Records contain fields that are related, such as a customer or an employee. Records and fields form the basis of all databases
- Degree: number of attributes in a table.
### Non-relational Databases
- What is NoSQL?: NoSQL is an approach to databases that represents a shift away from traditional relational database management systems (RDBMS). To define NoSQL, it is helpful to start by describing SQL, which is a query language used by RDBMS. Relational databases rely on tables, columns, rows, or schemas to organize and retrieve data. In contrast, NoSQL databases do not rely on these structures and use more flexible data models. 
- Types of NOSQL DB's: Key-value data stores, Document stores, Wide-column stores, Graph stores. 
- Benefits of NOSQL: 
    - Scalability 
    - Performance: By simply adding commodity resources, enterprises can increase performance with NoSQL databases. This enables organizations to continue to deliver reliably fast user experiences with a predictable return on investment for adding resources—again, without the overhead associated with manual sharding.
    - High Availability: NoSQL databases are generally designed to ensure high availability and avoid the complexity that comes with a typical RDBMS architecture that relies on primary and secondary nodes.
    - Global Availability: By automatically replicating data across multiple servers, data centers, or cloud resources, distributed NoSQL databases can minimize latency and ensure a consistent application experience wherever users are located
    - Flexible Data Modeling: NoSQL offers the ability to implement flexible and fluid data models
### Query for Data
- SQL Table Basics: 
Bit –Integer data with either a 1 or 0 value
Int –Integer (whole number) data from -2^31 (-2,147,483,648) through 2^31 – 1 (2,147,483,647)
Decimal –Fixed precision and scale numeric data from -10^38 -1 through 10^38
Timestamp –A database-wide unique number
Uniqueidentifier –A globally unique identifier (GUID)
Float –Floating precision number data from -1.79E + 308 through 1.79E + 308
Real –Floating precision number data from -3.40E + 38 through 3.40E + 38
Datetime –Date and time data from January 1, 1753, to December 31, 9999, with an accuracy of one-three-hundredths of a second, or 3.33 milliseconds
Char –Fixed-length non-Unicode character data with a maximum length of 8,000 characters
Varchar –Variable-length non-Unicode data with a maximum of 8,000 characters
Text –Variable-length non-Unicode data with a maximum length of 2^31 – 1 (2,147,483,647) characters
- A key that is used to uniquely identify a record in the database are called primary keys. These keys are used to relate information between two or more tables with foreign keys used to relate against a primary key.
### Choosing the Right Database Solution
- Relational DBs (SQL based): Let ’s say you have a table of students information, and a table of the course grades (course, grade, student id), every grade row relates to a student record.This DB consists of a collection of tables (like CSV tables), that are connected. 
- NoSQL DBs: NoSQL DBs there is no common structured schema for all records. Most of the NoSQL databases contain JSON records, and different records can include different fields.
 Amazon Relational Database Service (RDS): 
 - Amazon RDS is a managed relational database service that provides you six familiar database engines to choose from, including Amazon Aurora , MySQL  MariaDB , Oracle , Microsoft SQL Server , and PostgreSQL . This means that the code, applications, and tools you already use today with your existing databases can be used with Amazon RDS. Amazon RDS handles routine database tasks such as provisioning, patching, backup, recovery, failure detection, and repair.
 - What is an Amazon RDS DB Instance?:  A DB instance is an isolated database environment in the AWS Cloud. Your DB instance can contain multiple user-created databases.DB instance storage comes in three types: Magnetic, General Purpose (SSD), and Provisioned IOPS (PIOPS). They differ in performance characteristics and price, allowing you to tailor your storage performance and cost to the needs of your database. 
 When to Choose Amazon RDS: Use Amazon RDS when your application requires:
Complex transactions or complex queries
A medium to high query or write rate – up to 30,000 IOPS (15,000 reads + 15,000 writes)
No more than a single worker node or shard
High durability
Do not use RDS: 
Massive read/write rates (for example 150,000 writes per second)
Sharding due to high data size or throughput demands
Simple GET or PUT requests and queries that a NoSQL database can handle
Or, relational database management system (RDBMS) customization

### Amazon DynamoDB
- Amazon DynamoDB is a fully managed key-value and document NoSQL database service that provides fast and predictable performance with seamless scalability. DynamoDB lets you offload the administrative burdens of operating and scaling a distributed database so that you don't have to worry about hardware provisioning, setup and configuration, replication, software patching, or cluster scaling.
- Use Cases: Ad Technologies, Gaming, Retail. 
### Amazon Redshift
- Amazon Redshift is a fully managed, petabyte-scale data warehouse service in the cloud. You can start with just a few hundred gigabytes of data and scale to a petabyte or more. This enables you to use your data to acquire new insights and analytics for your business and customers.
- How Does Redshift Work?: Automation & Scaling... It is straightforward to automate most of the common administrative tasks to manage. Compatible...  Amazon Redshift supports standard SQL. It also provides high-performance Java Database Connectivity (JDBC) and Open Database Connectivity (ODBC) connectors. 
### Amazon Aurora
- Amazon Aurora is a MySQL and PostgreSQL-compatible relational database (Links to an external site.) built for the cloud, that combines the performance and availability of traditional enterprise databases with the simplicity and cost-effectiveness of open source databases. Using Amazon Aurora can reduce your database costs while improving the reliability and availability of the database
- Amazon Aurora is designed to be highly available: it stores multiple copies of your data across multiple Availability Zones with continuous backups to Amazon S3. 

#### __ TWO QUOTES I FOUND INTERESTING __ 
- "One of the benefits of a NoSQL database is that items in the same table can have different attributes. This gives you the flexibility to add attributes as your application evolves."
- " Amazon RDS enables you to focus on your application, so you can give applications the performance, high availability, security, and compatibility that they need. With Amazon RDS, your primary focus is your data and optimizing your application." 
#### __ FACTS I LEARNED __ 
- Difference between NoSQL and SQL DB's :  SQL  is associated with relational databases and is used to process structured database, while NoSQL databases are not relational. NoSQL databases are mostly document-oriented, non-structured and distributed. 
- I learned about Amazon Redshift, which is: Internet hosting service and data warehouse product. 
I still have a question about how the pricing model works for DynamoDB. Is it completely based off of how much you use (when it comes to Gb)? Or is it a flat rate that you pay monthly, or per entry? 

