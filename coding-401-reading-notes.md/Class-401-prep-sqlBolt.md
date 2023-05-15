# A Basic Guide to SQL 
## Created using [SQLBolt](https://sqlbolt.com/)

Select query with constraints
>SELECT column, another_column, …

>FROM mytable

> WHERE condition
    
    AND/OR another_condition
    AND/OR …;

Operators:
- =, !=, < <=, >, >=
- BETWEEN … AND …
- NOT BETWEEN … AND
- IN (…)
- NOT IN (…)

- LIKE
- NOT LIKE
- %
- _ 

All strings must be quoted

Select query with unique results

> SELECT DISTINCT column, another_column, …

> FROM mytable

> WHERE condition(s)

> ORDER BY column ASC/DESC

> LIMIT num_limit OFFSET num_offset


> INNER JOIN another_table
    
    > ON mytable.id = another_table.id

 - INNER/LEFT/RIGHT/FULL JOIN   

 - IS/NOT/NULL

 ### Queries with Expressions
 - Lesson 9-12 to ref directly per website

Insert statement with specific columns
 > INSERT INTO mytable

> (column, another_column, …)

> VALUES (value_or_expr, another_value_or_expr, …),
      (value_or_expr_2, another_value_or_expr_2, …),
      …;

Update statement with values

> UPDATE mytable

> SET column = value_or_expr, 
    other_column = another_value_or_expr, 
    …

> WHERE condition;

Delete statement with condition

> DELETE FROM mytable

> WHERE condition;

Create table statement w/ optional table constraint and default value

> CREATE TABLE IF NOT EXISTS mytable 

>(
    column DataType TableConstraint DEFAULT default_value,
    another_column DataType TableConstraint DEFAULT default_value,
    …
> );

Altering table to add new column(s)

> ALTER TABLE mytable

> ADD column DataType OptionalTableConstraint 
   
   >  DEFAULT default_value;

Altering table to remove column(s)

> ALTER TABLE mytable

> DROP column_to_be_deleted;

Altering table name

>ALTER TABLE mytable

>RENAME TO new_table_name;

Drop table statement

> DROP TABLE IF EXISTS mytable;

![SQL Tutorial Completion](/SQLtutorial(3).png "Certificate")