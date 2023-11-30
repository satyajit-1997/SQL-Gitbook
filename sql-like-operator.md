# SQL LIKE Operator

## <mark style="color:blue;">SQL LIKE Operator</mark>

**The LIKE operator is used in a WHERE clause to search for a specified pattern in a column.**

There are **two wildcards** often used in conjunction with the LIKE operator:

**- The percent sign (%) represents zero, one, or multiple characters**

**- The underscore sign (\_) represents one, single character**

The percent sign and the underscore can also be used in combinations

### <mark style="color:purple;">LIKE Syntax</mark>

```sql
SELECT column1, column2, ...
FROM table_name
  WHERE COLUMN LIKE pattern;
```

**Here are some examples showing different LIKE operators with '%' and '\_' wildcards:**

| LIKE Operator                   | Description                                                                  |
| ------------------------------- | ---------------------------------------------------------------------------- |
| WHERE first\_name LIKE 'a%'     | Finds any values that start with "a"                                         |
| WHERE first\_name LIKE '%a'     | Finds any values that end with "a"                                           |
| WHERE first\_name LIKE '%or%'   | Finds any values that have "or" in any position                              |
| WHERE first\_name LIKE '\_r%'   | Finds any values that have "r" in the second position                        |
| WHERE first\_name LIKE 'a\_%'   | Finds any values that start with "a" and are at least 2 characters in length |
| WHERE first\_name LIKE 'a\_\_%' | Finds any values that start with "a" and are at least 3 characters in length |
| WHERE first\_name LIKE 'a%o'    | Finds any values that start with "a" and ends with "o"                       |

### <mark style="color:purple;">SQL LIKE Examples</mark>

The following SQL statement selects all patients with a first\_name starting with "a":

```sql
SELECT * FROM patients
  WHERE first_name LIKE 'a%';
```

The following SQL statement selects all patients with a first\_name ending with "a":

```sql
SELECT * FROM patients
 WHERE first_name LIKE '%a';
```

The following SQL statement selects all patients with a first\_name that have "or" in any position:

```sql
SELECT * FROM patients
 WHERE first_name LIKE '%or%';
```

The following SQL statement selects all patients with a first\_name that have "r" in the second position:

```sql
SELECT * FROM patients
 WHERE first_name LIKE '_r%';
```

The following SQL statement selects all patients with a first\_name that starts with "a" and are at least 3 characters in length:

<pre class="language-sql"><code class="lang-sql">SELECT * FROM patients
<strong> WHERE first_name LIKE 'a__%';
</strong></code></pre>

The following SQL statement selects all patients with a first\_name that starts with "a" and ends with "o":

```sql
SELECT * FROM patients
 WHERE first_name LIKE 'a%o';
```

The following SQL statement selects all patients with a first\_name that does NOT start with "a":

```sql
SELECT * FROM patients
   WHERE first_name NOT LIKE 'a%';
```

```
```
