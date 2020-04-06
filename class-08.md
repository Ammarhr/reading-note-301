## SQL:

 ### What is SQL?
**SQL** stand for (**Structured Query Language**), is a language designed to allow both technical and non-technical users query, manipulate, and transform data from a relational database. And due to its simplicity, SQL databases provide safe and scalable storage for millions of websites and mobile applications.

**There are many popular SQL:** SQLite, MySQL, Postgres, Oracle and Microsoft SQL Server.

### Relational databases:
 **Relational databases** represents a collection of related (two-dimensional) tables. Each of the tables are similar to an Excel spreadsheet, with a fixed number of named columns (the attributes or properties of the table) and any number of rows of data.

### SELECT queries:
 To retrieve data from a SQL database, we need to write SELECT statements, which are often colloquially refered to as queries. A query in itself is just a statement which declares what data we are looking for, where to find it in the database, and optionally, how to transform it before it is returned.

***ex** Select query for a specific columns:

``
SELECT column, another_column, …
FROM mytable;
``
### Queries with constraints:

In order to filter certain results from being returned, we need to use a WHERE clause in the query.

**ex:** Select query with constraints:

```
SELECT column, another_column, …
FROM mytable
WHERE condition
    AND/OR another_condition
    AND/OR …;
```

>>
**note:** SQL doesn't require you to write the keywords all capitalized, but as a convention, it helps people distinguish SQL keywords from column and tables names, and makes the query easier to read.
>>

When writing WHERE clauses with columns containing text data, **SQL** supports a number of useful operators to do things like case-insensitive string comparison and wildcard pattern matching. like:
|         |                                                                    |                         |
|-------- | ------------------------------------------------------------------ | -----------------------:|
|=	| Case sensitive exact string comparison (notice the single equals)  | col_name = "abc"        |
|!= or <>	| Case sensitive exact string inequality   comparison	         | col_name != "abcd"      |
|LIKE	| Case insensitive exact string comparison	                   | col_name LIKE "ABC"     |
|NOT LIKE	| Case insensitive exact string inequality comparison	         | col_name NOT LIKE "ABCD"|

 **and more..**

>>
**note**: All strings must be quoted so that the query parser can distinguish words in the string from SQL keywords.
>>

### Filtering and sorting Query results:
**SQL** provides a convenient way to discard rows that have a duplicate column value by using the DISTINCT keyword.

**ex**:Select query with unique results:
```
SELECT DISTINCT column, another_column, …
FROM mytable
WHERE condition(s);
```

### Ordering results:
**SQL** provides a way to sort your results by a given column in ascending or descending order using the ORDER BY clause.

**ex**Select query with ordered results:
```
SELECT column, another_column, …
FROM mytable
WHERE condition(s)
ORDER BY column ASC/DESC;
```

