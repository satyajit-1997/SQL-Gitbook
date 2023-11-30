# SQL WHERE Clause

## <mark style="color:blue;">SQL WHERE Clause</mark>

**The WHERE clause is used to filter records.**

It is used to extract only those records that fulfill a specified condition.

```sql
SELECT column1, column2, ...
  FROM tablename
  WHERE condition;
```

### <mark style="color:purple;">WHERE Clause Example</mark>

The following SQL statement selects all the patients with the gender "F", in the "patients" table:

```sql
SELECT * FROM patients
WHERE gender ='F';
```

### <mark style="color:purple;">Text Fields vs. Numeric Fields</mark>

SQL requires single quotes around text values (most database systems will also allow double quotes).

However, numeric fields should not be enclosed in quotes:

```sql
SELECT * FROM patients
  WHERE patient_id=1;
```

### <mark style="color:purple;">Operators</mark>

**The following operators can be used in the WHERE clause:**

**Equal, =**

```sql
SELECT * FROM patients
 WHERE patient_id = 1;
```

**Greater Than, >**

```sql
SELECT * FROM patients
 WHERE patient_id > 5;
```

**Less Than, <**

```sql
SELECT * FROM patients
 WHERE patient_id < 5;
```

**Greater Than Or Equal To, >=**

```sql
SELECT * FROM patients
 WHERE patient_id >= 5;
```

**Less Than Or Equal To, <=**

```sql
SELECT * FROM patients
  WHERE patient_id <= 5;
```

**Not Equal, <> or != depending on sql version**

```sql
SELECT * FROM patients
 WHERE patient_id <> 5;
  -- No patient_id 5 row
```

**Between, inclusive range**

```sql
SELECT * FROM patients
 WHERE patient_id BETWEEN 4 AND 6;
```

**Like, pattern search**

```sql
SELECT * FROM patients
 WHERE first_name LIKE 'a%';
  -- First names starting with 'a'.
  -- View sql patterns for more info.
```

**In, in a collection**

```sql
SELECT * FROM patients
  WHERE patient_id IN (1,3,6,9);
  -- the values can be replaced with a sub-query.
```
