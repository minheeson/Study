##SQL

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



