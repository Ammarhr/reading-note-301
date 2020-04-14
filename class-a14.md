## Database Normalization
**Database normalization** is a process used to organize a database into tables and columns.  

- By limiting a table to one purpose you reduce the number of duplicate data contained within your database. This eliminates some issues stemming from database modifications.

- To achieve these objectives, we’ll use some established rules. As you apply these rules, new tables are formed. The progression from unruly to optimized passes through several normal forms.

### Why Database Normalization:
There are three main reasons to normalize a database:
1. The first is to minimize duplicate data.
2. minimize or avoid data modification issues.
3. simplify queries.

### Data Duplication and Modification Anomalies:
Duplicated information presents two problems:

- It increases storage and decrease performance.
- It becomes more difficult to maintain data changes.

#### Insert Anomaly
There are facts we cannot record until we know information for the entire row. 

####  Update Anomaly
In this case we have the same information in several rows. For instance if the office number changes, then there are multiple updates that need to be made.  If we don’t update all rows, then inconsistencies appear.
Deletion of a row causes removal of more than one set of facts. 

####  Search and Sort Issues
The last reason is making it easier to search and sort your data.

#### Definition of Database Normalization
There are three common forms of database normalization: 1st, 2nd, and 3rd normal form. They are also abbreviated as 1NF, 2NF, and 3NF respectively. 

1. The information is stored in a relational table with each column containing atomic values. There are no repeating groups of columns.
2. The table is in first normal form and all the columns depend on the table’s primary key.
3. the table is in second normal form and all of its columns are not transitively dependent on the primary key


