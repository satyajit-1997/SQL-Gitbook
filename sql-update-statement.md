# SQL UPDATE Statement

## <mark style="color:blue;">SQL UPDATE Statement</mark>

**The UPDATE statement is used to modify the existing records in a table.**

### <mark style="color:purple;">UPDATE Syntax</mark>

```sql
    UPDATE tablename
    SET column1 = value1, column2 = value2, ...
    WHERE condition;
```

Note: Be sure to specify the where clause. Failing to include the where clause will result in all of the rows to be updated.

The following SQL statement updates the first patient (patient\_id = 1) with a new first\_name and a new weight.

```sql
UPDATE patients
SET
  first_name = 'John',
  weight = 120
WHERE patient_id = 1;

-- display the patient we just updated
select * from patients where patient_id = 1

```

### <mark style="color:purple;">UPDATE Multiple Records</mark>

It is the WHERE clause that determines how many records will be updated.

The following SQL statement will update the allergies to 'NKA' (no known allergies) for all records where allergies is NULL

```sql
UPDATE patients
SET allergies = 'NKA'
WHERE allergies is NULL;

-- display the patients table
select * from patients;
```
