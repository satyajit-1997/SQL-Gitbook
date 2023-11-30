# SQL SELECT Statement

## <mark style="color:blue;">SQL SELECT Statement</mark>

The SELECT statement is used to select data from a database.

The data returned is stored in a result table, called the result-set.

### <mark style="color:purple;">SELECT Syntax</mark>

```sql
SELECT column1, column2, ...
 FROM tablename;
```

Here, column1, column2, ... are the field names of the table you want to select data from.&#x20;

If you want to **select all the fields** available in the table,&#x20;

use the following syntax:

```sql
SELECT * FROM tablename;
```

### <mark style="color:purple;">SELECT Column Example</mark>

The following SQL statement selects the "first\_name" and "last\_name" columns from the "patients" table:

```sql
SELECT first_name, last_name FROM patients;
```

### <mark style="color:purple;">SELECT \* Example</mark>

The following SQL statement selects all the columns from the "patients" table:

```sql
SELECT * FROM patients;
```
