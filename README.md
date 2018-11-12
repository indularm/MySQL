# MySQL

**Introduction**

The MySQL is one of the widly used database APIs that is powerful and robust and can be used for handling huge data sets fast and easy. The Pandas library can handle huge number of rows but not large number of columns and is slow when handling huge files. Therefore compared to that MySQL can achieve fast and organized data handling easily. 

Here first we'll discuss the basics of MySQL with examples and then discuss MySQL connector/Python so you can handle data within your Python code. 

**Basics of MySQL**

*What's a Database :* It's a collection of data with a methodology for accessing and handling the data. MySQL is the Database Management System (DBMS) that we use here to handle and access data. It sits inbetween the database and the user. SQL is the language that we'll use here to do the handling the way we want. There is a standard for SQL which is accepted by the industry and hence almost all the DBMS work on this standard SQL.

To see the current databases, 

```mysql
show databases
```
result will be as follows,

<img src="Figure_2.png" alt="blobs" class="inline"/>

To create a database, 

```mysql
CREATE DATABASE hello_world_db
```




