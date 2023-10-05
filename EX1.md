# EXP NO 1: DATA DEFINITION LANGUGE COMMANDS IN RDBMS

## AIM:
To create a student database and execute DDL queries using SQL.


## DDL (Data Definition Language)
<div align="justify">
DDL or Data Definition Language actually consists of the SQL commands that can be used to define the database schema. It simply deals with descriptions of the database schema and is used to create and modify the structure of database objects in the database. DDL is a set of SQL commands used to create, modify, and delete database structures but not data. These commands are normally not used by a general user, who should be accessing the database via an application.
</div>
 
## List of DDL commands: 
<div align="justify">
CREATE: This command is used to create the database or its objects (like table, index, function, views, store procedure, and triggers).
DROP: This command is used to delete objects from the database.
ALTER: This is used to alter the structure of the database.
TRUNCATE: This is used to remove all records from a table, including all spaces allocated for the records are removed.
RENAME: This is used to rename an object existing in the database.
</div>

## Query:
### 1) Create a table student with the following fieds rollno,name,age,address,phoneno.

### SQL QUERY: 
```
CREATE TABLE student(
    rollno numeric(5),name char(50),age numeric(5),
    address varchar(100),
    phoneno numeric(10)
    );
```


### OUTPUT:
![image](https://github.com/kabilan22000284/G2_DBMS/assets/123469171/52c4ce56-f11b-44c3-99ab-c677444673ee)


### 2) Change the above student table by adding another attribute department

### SQL QUERY: 
```
ALTER TABLE student ADD Department char(10);
```

### OUTPUT:
![image](https://github.com/kabilan22000284/G2_DBMS/assets/123469171/60750227-fef9-4fbb-a65d-c3025cd57bd0)




### 3) Drop the student table
 
### SQL QUERY: 
```
DROP TABLE student;
```


### OUTPUT:
![image](https://github.com/kabilan22000284/G2_DBMS/assets/123469171/e92140b6-49a0-4322-aacc-c6f9c6ad671d)



### 4) Delete the student table using truncate keyword

### SQL QUERY: 
```
TRUNCATE TABLE student;
```


### OUTPUT:
![image](https://github.com/kabilan22000284/G2_DBMS/assets/123469171/4ca9b2b3-a849-4999-8a8e-8e3d8484c175)




### 5) Rename the student table to mystudent

### SQL QUERY: 
```
ALTER TABLE student RENAME TO mystudent;
```


### OUTPUT:
![image](https://github.com/kabilan22000284/G2_DBMS/assets/123469171/9fb12096-2667-42ce-8ec4-85f80521cfca)

### RESULT:
Thus a student database has been created and DDL queries are executed successfully.
