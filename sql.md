## SQL

#### SELECT

~~~sql
SELECT column1, column2, ...(*)
FROM table_name;
~~~

#### WHERE

~~~sql
SELECT column1, column2, ...
FROM table_name
WHERE condition;
~~~

#### AND OR NOT

~~~sql
SELECT column1, column2, ...
FROM table_name
WHERE condition1 AND(OR) condition2;
~~~

~~~sql
SELECT column1, column2, ...
FROM table_name
WHERE NOT condition;
~~~

#### ORDER BY

~~~sql
SELECT column1, column2, ...
FROM table_name
ORDER BY column1, column2, ... ASC|DESC;
~~~

#### INSERT INTO

~~~sql
INSERT INTO table_name (column1, column2, column3, ...)
VALUES (value1, value2, value3, ...);
~~~

#### NULL VALUES

~~~sql
SELECT column_names
FROM table_name
WHERE column_name IS (NOT) NULL;
~~~

#### UPDATE

~~~sql
UPDATE table_name
SET column1 = value1, column2 = value2, ...
WHERE condition;
~~~

#### DELETE

~~~sql
DELETE FROM table_name WHERE condition;
~~~

#### MIN MAX

~~~sql
SELECT MIN(column_name)
FROM table_name
WHERE condition;
~~~

#### COUNT AVG SUM

~~~sql
SELECT COUNT(column_name)
FROM table_name
WHERE condition;
~~~
~~~sql
SELECT AVG(column_name)
FROM table_name
WHERE condition;
~~~
~~~sql
SELECT SUM(column_name)
FROM table_name
WHERE condition;
~~~

#### LIKE

~~~sql
SELECT column1, column2, ...
FROM table_name
WHERE columnN LIKE pattern; /* wildcards : %, _ */
~~~

#### IN

~~~sql
SELECT column_name(s)
FROM table_name
WHERE column_name IN (value1, value2, ...);
~~~
~~~sql
SELECT column_name(s)
FROM table_name
WHERE column_name IN (SELECT STATEMENT);
~~~

#### BETWEEN

~~~sql
SELECT column_name(s)
FROM table_name
WHERE column_name BETWEEN value1 AND value2;
~~~

#### ALIAS

~~~sql
SELECT column_name AS alias_name
FROM table_name;
~~~

#### JOIN

~~~sql
SELECT Orders.OrderID, Customers.CustomerName, Orders.OrderDate
FROM Orders
INNER JOIN Customers ON Orders.CustomerID=Customers.CustomerID;
~~~

#### INNER JOIN

~~~sql
SELECT column_name(s)
FROM table1
INNER JOIN table2 ON table1.column_name = table2.column_name;
~~~

#### LEFT JOIN

~~~sql
SELECT column_name(s)
FROM table1
LEFT JOIN table2 ON table1.column_name = table2.column_name;
~~~

#### RIGHT JOIN

~~~sql
SELECT column_name(s)
FROM table1
RIGHT JOIN table2 ON table1.column_name = table2.column_name;
~~~

#### FULL OUTER JOIN

~~~sql
SELECT column_name(s)
FROM table1
FULL OUTER JOIN table2 ON table1.column_name = table2.column_name;
~~~

#### SELF JOIN 

~~~sql
SELECT column_name(s)
FROM table1 T1, table1 T2
WHERE condition;
~~~

#### UNION 

~~~sql
SELECT column_name(s) FROM table1
UNION (ALL)
SELECT column_name(s) FROM table2;
~~~

#### GROUP BY

~~~sql
SELECT column_name(s)
FROM table_name
WHERE condition
GROUP BY column_name(s)
ORDER BY column_name(s);
~~~

#### HAVING 

~~~sql
SELECT column_name(s)
FROM table_name
WHERE condition
GROUP BY column_name(s)
HAVING condition
ORDER BY column_name(s);
~~~

#### EXISTS 

~~~sql
SELECT column_name(s)
FROM table_name
WHERE EXISTS
(SELECT column_name FROM table_name WHERE condition);
~~~

#### ANY ALL

~~~sql
SELECT column_name(s)
FROM table_name
WHERE column_name operator ANY(ALL)
(SELECT column_name FROM table_name WHERE condition);
~~~

#### CASE

~~~sql
CASE
    WHEN condition1 THEN result1
    WHEN condition2 THEN result2
    WHEN conditionN THEN resultN
    ELSE result
END;
~~~

#### PROCEDURE

~~~sql
CREATE PROCEDURE procedure_name
AS
sql_statement
GO;
~~~
~~~sql
EXEC procedure_name;
~~~




