# SQL DELETE Statement

## <mark style="color:blue;">SQL DELETE Statement</mark>

**The DELETE statement is used to delete existing records in a table.**

### <mark style="color:purple;">DELETE Syntax</mark>

```sql
DELETE FROM tablename WHERE condition;
```

Note: Be sure to specify the where clause. Failing to include the where clause will result in all of the rows to be deleted.

### <mark style="color:purple;">SQL DELETE Example</mark>

The following SQL statement deletes all patients named "Paul" from the "patients" table:

```sql
DELETE FROM patients WHERE first_name = 'Paul';

-- There are no longer any patients named 'Paul' in the database
select * from patients where first_name = 'P-- Insert a record
INSERT INTO patients (first_name, last_name, gender)
    VALUES ('Jane', 'Doe','F');
    
-- Select the most recent record by id to display it.
select * from patients
	where patient_id = (select max(patient_id) from patients);aul'
```
