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
WHERE columnN LIKE pattern; /** wildcards : %, _ **/
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
