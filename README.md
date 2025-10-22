# Experiment 3: DML Commands

## AIM
To study and implement DML (Data Manipulation Language) commands.

## THEORY

### 1. INSERT INTO
Used to add records into a relation.
These are three type of INSERT INTO queries which are as
A)Inserting a single record
**Syntax (Single Row):**
```sql
INSERT INTO table_name (field_1, field_2, ...) VALUES (value_1, value_2, ...);
```
**Syntax (Multiple Rows):**
```sql
INSERT INTO table_name (field_1, field_2, ...) VALUES
(value_1, value_2, ...),
(value_3, value_4, ...);
```
**Syntax (Insert from another table):**
```sql
INSERT INTO table_name SELECT * FROM other_table WHERE condition;
```
### 2. UPDATE
Used to modify records in a relation.
Syntax:
```sql
UPDATE table_name SET column1 = value1, column2 = value2 WHERE condition;
```
### 3. DELETE
Used to delete records from a relation.
**Syntax (All rows):**
```sql
DELETE FROM table_name;
```
**Syntax (Specific condition):**
```sql
DELETE FROM table_name WHERE condition;
```
### 4. SELECT
Used to retrieve records from a table.
**Syntax:**
```sql
SELECT column1, column2 FROM table_name WHERE condition;
```
**Question 1**
--
<img width="1047" height="659" alt="image" src="https://github.com/user-attachments/assets/4303af56-0bb6-41ae-bc0f-f313eeded779" />


```sql
update Employees
set hire_date='2024-01-24' 
WHERE DEPARTMENT_ID=50 
```

**Output:**

<img width="1211" height="303" alt="image" src="https://github.com/user-attachments/assets/110fa614-7284-435e-8610-f322ad16aea6" />


**Question 2**
---
<img width="1237" height="328" alt="image" src="https://github.com/user-attachments/assets/bd0f60f5-14ad-4bc5-ac35-5a531eec9870" />


```sql
update Products
set product_name ='Premium Bread'
where product_ID =5
```

**Output:**

<img width="1251" height="416" alt="image" src="https://github.com/user-attachments/assets/989042fc-f746-4b15-8bb2-9b1f24ce0642" />

**Question 3**
---
<img width="1237" height="628" alt="image" src="https://github.com/user-attachments/assets/8f8ac8f5-7842-4120-8670-7a8a29fa5717" />


```sql
UPDATE products
SET reorder_lvl = reorder_lvl * 0.7
WHERE product_name LIKE '%cream%'
  AND quantity > reorder_lvl;
```

**Output:**

<img width="1165" height="517" alt="image" src="https://github.com/user-attachments/assets/d81a2699-eab1-45c5-8475-07c4dfcb10d7" />

**Question 4**
---
<img width="1127" height="680" alt="image" src="https://github.com/user-attachments/assets/7fb4a92f-66ae-4ce4-83ec-f85231141c55" />


```sql
update Employees
set email= 'Unavailable'
```

**Output:**

<img width="1191" height="458" alt="image" src="https://github.com/user-attachments/assets/d261c511-f263-4dfa-a197-c5b11e9447e1" />

**Question 5**
---
<img width="1228" height="486" alt="image" src="https://github.com/user-attachments/assets/a8c20d67-781c-492b-8822-229df6d5101c" />


```sql
delete from customer
where GRADE%2!=0
```

**Output:**

<img width="1192" height="432" alt="image" src="https://github.com/user-attachments/assets/69ceb6d2-f83f-4d25-b20c-54316b46febd" />

**Question 6**
---
<img width="1023" height="161" alt="image" src="https://github.com/user-attachments/assets/5d2b4420-c82e-4ff1-abdb-443813a5f32a" />


```sql
delete from Doctors 
where specialization IS('Cardiology')
```

**Output:**

<img width="1187" height="381" alt="image" src="https://github.com/user-attachments/assets/a9b7de85-1081-4af8-8e52-737482aa0391" />


**Question 7**
---
<img width="1217" height="727" alt="image" src="https://github.com/user-attachments/assets/6a110848-31d0-473a-aeb2-50629592efc2" />


```sql
DELETE FROM customer
WHERE CUST_NAME LIKE '______';

```

**Output:**

<img width="1162" height="701" alt="image" src="https://github.com/user-attachments/assets/87604b9e-66f5-4596-8661-681ab7f6b111" />


**Question 8**
---
<img width="1225" height="702" alt="image" src="https://github.com/user-attachments/assets/bc02eeda-1d86-428b-9b70-0e6af7b96d79" />

```sql
Delete from customer where GRADE< 2
```

**Output:**

<img width="886" height="553" alt="image" src="https://github.com/user-attachments/assets/37109f6c-e023-4a8e-81d7-18ccba4a5777" />

**Question 9**
---
<img width="1037" height="497" alt="image" src="https://github.com/user-attachments/assets/bc3998bf-0d2f-43d2-8a83-621fe3c5fba6" />


```sql
select *
from EmployeeInfo 
order by EmpID DESC
limit 5
```

**Output:**

<img width="1212" height="372" alt="image" src="https://github.com/user-attachments/assets/7cb7429e-4a14-4d1e-b5bb-e97ea180471d" />

**Question 10**
---
<img width="1025" height="677" alt="image" src="https://github.com/user-attachments/assets/da2c326f-2259-4837-a3d0-e650a11c072b" />


```sql
SELECT *
FROM EmployeePosition
WHERE strftime('%Y', DateOfJoining) = '2020';
```

**Output:**

<img width="1157" height="316" alt="image" src="https://github.com/user-attachments/assets/9cfb5449-d181-4bcb-abf5-8970504337ce" />


## RESULT
Thus, the SQL queries to implement DML commands have been executed successfully.
](https://github.com/swathisiva212/EXP-2-dbms)
