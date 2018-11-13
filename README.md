# MySQL

**Introduction**

The MySQL is one of the widly used database APIs that is powerful and robust and can be used for handling huge data sets fast and easy. The Pandas library can handle huge number of rows but not large number of columns and is slow when handling huge files. Therefore compared to that MySQL can achieve fast and organized data handling easily. 

Here first we'll discuss the basics of MySQL with examples and then discuss MySQL connector/Python so you can handle data within your Python code. 

**Basics of MySQL**

*What's a Database :* It's a collection of data with a methodology for accessing and handling the data. MySQL is the Database Management System (DBMS) that we use here to handle and access data. It sits inbetween the database and the user. SQL is the language that we'll use here to do the handling the way we want. There is a standard for SQL which is accepted by the industry and hence almost all the DBMS work on this standard SQL.

To see the current databases, 

```mysql
SHOW DATABASES
```
result will be as follows,

<img src="Figure_2.png" alt="blobs" class="inline"/>

To create a database, 

```mysql
CREATE DATABASE hello_world_db
```
result will be as follows, 
  
<img src="Figure_2.png" alt="blobs" class="inline"/>

To delete a database, 

```mysql
DROP DATABASE hello_world_db
```
result will be as follows, 

<img src="Figure_2.png" alt="blobs" class="inline"/>

To tell the DBMS which database that we're woking with,

```mysql 
USE soap_store
```
result will be as follows, 

<img src="Figure_2.png" alt="blobs" class="inline"/>

Another similar command is, 

```mysql
SELECT database()
```
result will tell you the database that you're currently working on is the SELECTed databse, 

<img src="Figure_2.png" alt="blobs" class="inline"/>

Databse is made up of set of tables. That's what we use to store the data, 

Hence we'll see how to create the tables, 

```mysql 
CREATE TABLE tablename
  (
    column_name data_type, 
    column_name data_type
  );
```
example, 

```mysql 
CREATE TABLE soap_sales
  (
    item_code INT,
    item_name VARCHAR
  );
```
result is as follows, 

<img src="Figure_2.png" alt="blobs" class="inline"/>
  
To see the created table, 

```mysql 
SHOW TABLES
```

result is as follows, 

<img src="Figure_2.png" alt="blobs" class="inline"/>

we can also view columns from a particular table, 

```mysql
SHOW COLUMNS FROM soap_sales
```
OR

```mysql
DESC soap_sales
```

result is as follows, 

<img src="Figure_2.png" alt="blobs" class="inline"/>

To delete a table, 

```mysql
DROP TABLE <table_name>
```
result is as follows, 

<img src="Figure_2.png" alt="blobs" class="inline"/>

Now let's see how to put data into the tables, 

```mysql 
INSERT INTO soap_sales(item_codes, name)
VALUES(150487, 'Pumpkin');
```
now we can view data present in the table, 

<img src="Figure_2.png" alt="blobs" class="inline"/>

Remeber that the order of entering data matters and should be entered in the order of field names, 

To see the data entered you can do the following, 

```mysql
SELECT * FROM soap_sales
```

result will be as follows, 

<img src="Figure_2.png" alt="blobs" class="inline"/>





