# EX-3-SubQueries-Views-and-Joins
# DATE:
#   Create employee Table
CREATE TABLE EMP (EMPNO NUMBER(4) PRIMARY KEY,ENAME VARCHAR2(10),JOB VARCHAR2(9),MGR NUMBER(4),HIREDATE DATE,SAL NUMBER(7,2),COMM NUMBER(7,2),DEPTNO NUMBER(2));
# Insert the values
INSERT INTO EMP (EMPNO, ENAME, JOB, MGR, HIREDATE, SAL, COMM, DEPTNO) VALUES (7369, 'SMITH', 'CLERK', 7902, '17-DEC-80', 800, NULL, 20); INSERT INTO EMP (EMPNO, ENAME, JOB, MGR, HIREDATE, SAL, COMM, DEPTNO) VALUES (7499, 'ALLEN', 'SALESMAN', 7698, '20-FEB-81', 1600, 300, 30); INSERT INTO EMP (EMPNO, ENAME, JOB, MGR, HIREDATE, SAL, COMM, DEPTNO) VALUES (7521, 'WARD', 'SALESMAN', 7698, '22-FEB-81', 1250, 500, 30); INSERT INTO EMP (EMPNO, ENAME, JOB, MGR, HIREDATE, SAL, COMM, DEPTNO) VALUES (7566, 'JONES', 'MANAGER', 7839, '02-APR-81', 2975, NULL, 20); INSERT INTO EMP (EMPNO, ENAME, JOB, MGR, HIREDATE, SAL, COMM, DEPTNO) VALUES (7654, 'MARTIN', 'SALESMAN', 7698, '28-SEP-81', 1250, 1400, 30); INSERT INTO EMP (EMPNO, ENAME, JOB, MGR, HIREDATE, SAL, COMM, DEPTNO) VALUES (7934, 'MILLER', 'CLERK', 7782, TO_DATE('23-JAN-82', 'DD-MON-RR'), 1300, 10, 10);

## Create department table
```sql
CREATE TABLE DEPT (DEPTNO NUMBER(2) PRIMARY KEY,DNAME VARCHAR2(14),LOC VARCHAR2(13));
```
## Insert the values in the department table
INSERT INTO DEPT (DEPTNO, DNAME, LOC) VALUES (10, 'ACCOUNTING', 'NEW YORK');
INSERT INTO DEPT (DEPTNO, DNAME, LOC) VALUES (20, 'RESEARCH', 'DALLAS');
INSERT INTO DEPT (DEPTNO, DNAME, LOC) VALUES (30, 'SALES', 'CHICAGO');
INSERT INTO DEPT (DEPTNO, DNAME, LOC) VALUES (40, 'OPERATIONS', 'BOSTON');
### Q1) List the name of the employees whose salary is greater than that of employee with empno 7566.
## QUERY:
![image](https://github.com/imthiyas19/EX-3-SubQueries-Views-and-Joins/assets/120353416/298f74f1-b49e-46a3-a233-b635fe48268b)
## OUTPUT:
![image](https://github.com/imthiyas19/EX-3-SubQueries-Views-and-Joins/assets/120353416/897318a0-0ada-4731-a3fb-cfebed1d09ed)
### Q2) List the ename,job,sal of the employee who get minimum salary in the company.
## QUERY:
![image](https://github.com/imthiyas19/EX-3-SubQueries-Views-and-Joins/assets/120353416/4fef5e45-c3ee-45bd-8e12-8274146ca77f)
## OUTPUT
![image](https://github.com/imthiyas19/EX-3-SubQueries-Views-and-Joins/assets/120353416/4c31ca41-7bfa-492d-9752-0ec2b1fcec8e)
## Q3) List ename, job of the employees who work in deptno 10 and his/her job is any one of the job in the department ‘SALES’.
## QUERY:
![image](https://github.com/imthiyas19/EX-3-SubQueries-Views-and-Joins/assets/120353416/b733e9f8-2e1e-4ab4-a5d5-5ed483ff98c7)
## OUTPUT:
![image](https://github.com/imthiyas19/EX-3-SubQueries-Views-and-Joins/assets/120353416/15058445-32c0-4c1a-b872-adb1136bf592)
## Q4) Create a view empv5 (for the table emp) that contains empno, ename, job of the employees who work in dept 10.
# QUERY:
![image](https://github.com/imthiyas19/EX-3-SubQueries-Views-and-Joins/assets/120353416/1ff470b4-1d37-457a-8add-6626c8c9dc09)


## OUTPUT:
![image](https://github.com/imthiyas19/EX-3-SubQueries-Views-and-Joins/assets/120353416/2f50baf5-d203-4769-bd6b-d1a5584b8977)


## Q5) Create a view with column aliases empv30 that contains empno, ename, sal of the employees who work in dept 30. Also display the contents of the view.
## QUERY:
![image](https://github.com/imthiyas19/EX-3-SubQueries-Views-and-Joins/assets/120353416/faff820d-f1b0-4344-9a3b-4ad407277d78)


## OUTPUT:
![image](https://github.com/imthiyas19/EX-3-SubQueries-Views-and-Joins/assets/120353416/72c73d59-c80e-4a40-a02f-042f1e3ea3a3)


Q6) Update the view empv5 by increasing 10% salary of the employees who work as ‘CLERK’. Also confirm the modifications in emp table
# QUERY:
![image](https://github.com/imthiyas19/EX-3-SubQueries-Views-and-Joins/assets/120353416/a4f62e08-13b9-4b9f-8dcc-b84ad0b189aa)


# OUTPUT:
![image](https://github.com/imthiyas19/EX-3-SubQueries-Views-and-Joins/assets/120353416/4692387a-4bb5-4bb2-9225-99813010549b)


# Create a Customer1 Table
INSERT INTO Salesman1 (salesman_id, name, city, commission) VALUES(5003, 'Lauson

# Q7) Write a SQL query to find the salesperson and customer who reside in the same city. Return Salesman, cust_name and city.
# QUERY:
![image](https://github.com/imthiyas19/EX-3-SubQueries-Views-and-Joins/assets/120353416/09327a73-a7a0-457d-b85a-1dbc71f99980)


# OUTPUT:
![image](https://github.com/imthiyas19/EX-3-SubQueries-Views-and-Joins/assets/120353416/607e5cc7-4da9-454a-8611-32174f1feac4)


# OUTPUT:
![image](https://github.com/imthiyas19/EX-3-SubQueries-Views-and-Joins/assets/120353416/61d10be6-2b07-4b2f-910a-9052aa1f9bed)


# Q9) Perform Natural join on both tables
# QUERY:
![image](https://github.com/imthiyas19/EX-3-SubQueries-Views-and-Joins/assets/120353416/ea1e6471-c657-4709-ad75-be4924ea0d97)


# OUTPUT:
![image](https://github.com/imthiyas19/EX-3-SubQueries-Views-and-Joins/assets/120353416/f0949ae6-85e9-4158-ae6f-2ea39e0d0531)


# Q10) Perform Left and right join on both tables
# QUERY:
# Left Join
![image](https://github.com/imthiyas19/EX-3-SubQueries-Views-and-Joins/assets/120353416/c79e33f8-6597-4400-bd94-af476bbf67da)


# OUTPUT:
# Left Join
![image](https://github.com/imthiyas19/EX-3-SubQueries-Views-and-Joins/assets/120353416/1ec48ce6-1825-42d4-ab58-d067ac342d0e)


# Right Join
![image](https://github.com/imthiyas19/EX-3-SubQueries-Views-and-Joins/assets/120353416/ab70b392-e6db-4d9e-970e-5c386be57c4d)
# RESULT:
Hence successfully created SubQueries, Views and Joins.











