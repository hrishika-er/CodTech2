Name:Hrishika Verma
Company:CodTech
ID:CT4SQL4338
Domain:SQL
Duration:july to August
MENTOR:Muzammil Ahmed
Overview Of the project
PROJECT:STUDENT  DATABASE MANAGEMENT SYSTEM
OBJECTIVE:
Create a database to manage student records, including 
personal details, courses, and grades. This project helps you 
practice creating and managing relational databases. Design 
tables for students, courses, and enrollments. Write SQL 
queries to manage student records. Implement joins to 
combine data from multiple tableS.
KEY ACTIVITIES:
1. Writing SQL queries to retrieve, manipulate, and analyze data from databases
2. Creating and modifying database tables, views, indexes, and other database objects
3. Optimizing SQL queries for performance by using appropriate indexing and query optimization techniques
4. Managing database security by setting permissions and access controls for users
5. Monitoring database performance and troubleshooting issues related to SQL queries and database operations
6. Working with stored procedures, functions, triggers, and other advanced SQL features to automate tasks or enforce business rules within the database system.
TECHNOLOGY USED:
* MYSQL
  
mysql> describe students;
+---------------+--------------+------+-----+---------+-------+
| Field         | Type         | Null | Key | Default | Extra |
+---------------+--------------+------+-----+---------+-------+
| student_id    | int(11)      | NO   | PRI | NULL    |       |
| first_name    | varchar(50)  | YES  |     | NULL    |       |
| last_name     | varchar(50)  | YES  |     | NULL    |       |
| date_of_birth | date         | YES  |     | NULL    |       |
| address       | varchar(100) | YES  |     | NULL    |       |
| phone_number  | varchar(15)  | YES  |     | NULL    |       |
+---------------+--------------+------+-----+---------+-------+
6 rows in set (0.02 sec)

Hrishika verma CA 1 MITM, [7/14/2024 4:11 PM]
mysql> insert into students(student_id,first_name,last_name,date_of_birth,address,phone_number) values(1004,"aditya","sharma","1996-08-07","diamonds",59897895);
Query OK, 1 row affected (0.00 sec)

mysql> insert into students(student_id,first_name,last_name,date_of_birth,address,phone_number) values(1005,"aditi","sharma","1995-01-01","diamonds",598978395);
Query OK, 1 row affected (0.00 sec)

mysql> insert into students(student_id,first_name,last_name,date_of_birth,address,phone_number) values(1006,"pankaj","sony","1995-03-01","nanakheda",37749986);
Query OK, 1 row affected (0.00 sec)

mysql> insert into students(student_id,first_name,last_name,date_of_birth,address,phone_number) values(1007,"palak","sethi","1994-03-03","tajplaca",795734987);
Query OK, 1 row affected (0.00 sec)

mysql> select * from students;
+------------+------------+-----------+---------------+-------------+--------------+
| student_id | first_name | last_name | date_of_birth | address     | phone_number |
+------------+------------+-----------+---------------+-------------+--------------+
|       1001 | John       | Doe       | 1995-03-15    | 123 Main St | NULL         |
|       1002 | riya       | batra     | 1995-03-18    | 282 street  | 77972987     |
|       1003 | hrishika   | verma     | 1996-05-07    | tirupati    | 59597895     |
|       1004 | aditya     | sharma    | 1996-08-07    | diamonds    | 59897895     |
|       1005 | aditi      | sharma    | 1995-01-01    | diamonds    | 598978395    |
|       1006 | pankaj     | sony      | 1995-03-01    | nanakheda   | 37749986     |
|       1007 | palak      | sethi     | 1994-03-03    | tajplaca    | 795734987    |
+------------+------------+-----------+---------------+-------------+--------------+
7 rows in set (0.00 sec)
Hrishika verma CA 1 MITM, [7/14/2024 4:11 PM]
mysql> describe students;
+---------------+--------------+------+-----+---------+-------+
| Field         | Type         | Null | Key | Default | Extra |
+---------------+--------------+------+-----+---------+-------+
| student_id    | int(11)      | NO   | PRI | NULL    |       |
| first_name    | varchar(50)  | YES  |     | NULL    |       |
| last_name     | varchar(50)  | YES  |     | NULL    |       |
| date_of_birth | date         | YES  |     | NULL    |       |
| address       | varchar(100) | YES  |     | NULL    |       |
| phone_number  | varchar(15)  | YES  |     | NULL    |       |
+---------------+--------------+------+-----+---------+-------+
6 rows in set (0.02 sec)

Hrishika verma CA 1 MITM, [7/14/2024 4:12 PM]
ysql> insert into course(cid,cname,instructor) values(2001,"btech","j.p joshi");
Query OK, 1 row affected (0.00 sec)

mysql> insert into course(cid,cname,instructor) values(2002,"bsc","johri");
Query OK, 1 row affected (0.00 sec)

mysql> insert into course(cid,cname,instructor) values(2003,"msc","johri");
Query OK, 1 row affected (0.00 sec)

mysql> insert into course(cid,cname,instructor) values(2004,"msc","keshav sharma");
Query OK, 1 row affected (0.00 sec)

mysql> insert into course(cid,cname,instructor) values(2005,"mca","kapil");
Query OK, 1 row affected (0.00 sec)

mysql> insert into course(cid,cname,instructor) values(2006,"bca","prerna");
Query OK, 1 row affected (0.00 sec)

Hrishika verma CA 1 MITM, [7/14/2024 4:13 PM]
mysql> select * from course;
+------+-------+---------------+
| cid  | cname | instructor    |
+------+-------+---------------+
| 2001 | btech | j.p joshi     |
| 2002 | bsc   | johri         |
| 2003 | msc   | johri         |
| 2004 | msc   | keshav sharma |
| 2005 | mca   | kapil         |
| 2006 | bca   | prerna        |
+------+-------+---------------+
6 rows in set (0.00 sec)
Hrishika verma CA 1 MITM, [7/14/2024 4:14 PM]
> insert into enrollement(237376767);
ERROR 1064 (42000): You have an error in your SQL syntax; check the manual that corresponds to your MySQL server version for the right syntax to use near '237376767)' at line 1
mysql> insert into enrollement(eid) values(10000010);
Query OK, 1 row affected (0.00 sec)

mysql> insert into enrollement(eid) values(10000011);
Query OK, 1 row affected (0.00 sec)

mysql> insert into enrollement(eid) values(10000012);
Query OK, 1 row affected (0.00 sec)

mysql> insert into enrollement(eid) values(10000013);
Query OK, 1 row affected (0.00 sec)

mysql> insert into enrollement(eid) values(10000014);
Query OK, 1 row affected (0.00 sec)

mysql> insert into enrollement(eid) values(10000015);
Query OK, 1 row affected (0.00 sec)

mysql> insert into enrollement(eid) values(10000016);
Query OK, 1 row affected (0.00 sec)

mysql> insert into enrollement(eid) values(10000017);
Query OK, 1 row affected (0.00 sec)

mysql> select * from enrollement;
+----------+
| eid      |
+----------+
| 10000010 |
| 10000011 |
| 10000012 |
| 10000013 |
| 10000014 |
| 10000015 |
| 10000016 |
| 10000017 |
+----------+

Hrishika verma CA 1 MITM, [7/14/2024 4:21 PM]
alter table students add cid int(50);
Query OK, 0 rows affected (0.13 sec)
Records: 0  Duplicates: 0  Warnings: 0

mysql> update students set cid="2001" where student_id="1001";
Query OK, 1 row affected (0.00 sec)
Rows matched: 1  Changed: 1  Warnings: 0

mysql> update students set cid="2002" where student_id="1002";
Query OK, 1 row affected (0.00 sec)
Rows matched: 1  Changed: 1  Warnings: 0

mysql> update students set cid="2003" where student_id="1003";
Query OK, 1 row affected (0.00 sec)
Rows matched: 1  Changed: 1  Warnings: 0

mysql> update students set cid="2004" where student_id="1004";
Query OK, 1 row affected (0.00 sec)
Rows matched: 1  Changed: 1  Warnings: 0

mysql> update students set cid="2005" where student_id="1005";
Query OK, 1 row affected (0.00 sec)
Rows matched: 1  Changed: 1  Warnings: 0
Hrishika verma CA 1 MITM, [7/14/2024 4:14 PM]
> insert into enrollement(237376767);
ERROR 1064 (42000): You have an error in your SQL syntax; check the manual that corresponds to your MySQL server version for the right syntax to use near '237376767)' at line 1
mysql> insert into enrollement(eid) values(10000010);
Query OK, 1 row affected (0.00 sec)

mysql> insert into enrollement(eid) values(10000011);
Query OK, 1 row affected (0.00 sec)

mysql> insert into enrollement(eid) values(10000012);
Query OK, 1 row affected (0.00 sec)

mysql> insert into enrollement(eid) values(10000013);
Query OK, 1 row affected (0.00 sec)

mysql> insert into enrollement(eid) values(10000014);
Query OK, 1 row affected (0.00 sec)

mysql> insert into enrollement(eid) values(10000015);
Query OK, 1 row affected (0.00 sec)

mysql> insert into enrollement(eid) values(10000016);
Query OK, 1 row affected (0.00 sec)

mysql> insert into enrollement(eid) values(10000017);
Query OK, 1 row affected (0.00 sec)

mysql> select * from enrollement;
+----------+
| eid      |
+----------+
| 10000010 |
| 10000011 |
| 10000012 |
| 10000013 |
| 10000014 |
| 10000015 |
| 10000016 |
| 10000017 |
+----------+

Hrishika verma CA 1 MITM, [7/14/2024 4:21 PM]
mysql> select * from students;
+------------+------------+-----------+---------------+-------------+--------------+------+
| student_id | first_name | last_name | date_of_birth | address     | phone_number | cid  |
+------------+------------+-----------+---------------+-------------+--------------+------+
|       1001 | John       | Doe       | 1995-03-15    | 123 Main St | 43893737     | 2001 |
|       1002 | riya       | batra     | 1995-03-18    | 282 street  | 77972987     | 2002 |
|       1003 | hrishika   | verma     | 1996-05-07    | tirupati    | 59597895     | 2003 |
|       1004 | aditya     | sharma    | 1996-08-07    | diamonds    | 59897895     | 2004 |
|       1005 | aditi      | sharma    | 1995-01-01    | diamonds    | 598978395    | 2005 |
|       1006 | pankaj     | sony      | 1995-03-01    | nanakheda   | 37749986     | 2006 |
|       1007 | palak      | sethi     | 1994-03-03    | tajplaca    | 795734987    | 2007 |
+------------+------------+-----------+---------------+-------------+--------------+------+
7 rows in set (0.00 sec)
LEFT JOIN

mysql> select s.first_name,s.last_name,c.cname,c.instructor from students s  left join course c  on s.cid=c.cid;
+------------+-----------+---------+---------------+
| first_name | last_name | cname   | instructor    |
+------------+-----------+---------+---------------+
| John       | Doe       | btech   | j.p joshi     |
| riya       | batra     | bsc     | johri         |
| hrishika   | verma     | mpharma | johri         |
| aditya     | sharma    | msc     | keshav sharma |
| aditi      | sharma    | mca     | kapil         |
| pankaj     | sony      | bca     | prerna        |
| palak      | sethi     | NULL    | NULL          |
+------------+-----------+---------+---------------+
7 rows in set (0.00 sec)

RIGHT JOIN

mysql> select s.first_name,s.last_name,c.cname,c.instructor from students s  right join course c  on s.cid=c.cid;
+------------+-----------+---------+---------------+
| first_name | last_name | cname   | instructor    |
+------------+-----------+---------+---------------+
| John       | Doe       | btech   | j.p joshi     |
| riya       | batra     | bsc     | johri         |
| hrishika   | verma     | mpharma | johri         |
| aditya     | sharma    | msc     | keshav sharma |
| aditi      | sharma    | mca     | kapil         |
| pankaj     | sony      | bca     | prerna        |
+------------+-----------+---------+---------------+
6 rows in set (0.00 sec)

SELF JOIN

mysql> select c.cname,c.cid,p.instructor from course c, course p where c.cid=p.cid;
+---------+------+---------------+
| cname   | cid  | instructor    |
+---------+------+---------------+
| btech   | 2001 | j.p joshi     |
| bsc     | 2002 | johri         |
| mpharma | 2003 | johri         |
| msc     | 2004 | keshav sharma |
| mca     | 2005 | kapil         |
| bca     | 2006 | prerna        |
+---------+------+---------------+
6 rows in set (0.00 sec)

CROSS JOIN

mysql> select s.first_name,e.eid,e.cid,s.address,s.phone_number from students s cross join enrollement  e;
+------------+----------+------+-------------+--------------+
| first_name | eid      | cid  | address     | phone_number |
+------------+----------+------+-------------+--------------+
| John       | 10000010 | 2001 | 123 Main St | 43893737     |
| riya       | 10000010 | 2001 | 282 street  | 77972987     |
| hrishika   | 10000010 | 2001 | tirupati    | 59597895     |
| aditya     | 10000010 | 2001 | diamonds    | 59897895     |
| aditi      | 10000010 | 2001 | diamonds    | 598978395    |
| pankaj     | 10000010 | 2001 | nanakheda   | 37749986     |
| palak      | 10000010 | 2001 | tajplaca    | 795734987    |
| John       | 10000011 | 2002 | 123 Main St | 43893737     |
| riya       | 10000011 | 2002 | 282 street  | 77972987     |
| hrishika   | 10000011 | 2002 | tirupati    | 59597895     |
| aditya     | 10000011 | 2002 | diamonds    | 59897895     |
| aditi      | 10000011 | 2002 | diamonds    | 598978395    |
| pankaj     | 10000011 | 2002 | nanakheda   | 37749986     |
| palak      | 10000011 | 2002 | tajplaca    | 795734987    |
| John       | 10000012 | 2003 | 123 Main St | 43893737     |
| riya       | 10000012 | 2003 | 282 street  | 77972987     |
| hrishika   | 10000012 | 2003 | tirupati    | 59597895     |
| aditya     | 10000012 | 2003 | diamonds    | 59897895     |
| aditi      | 10000012 | 2003 | diamonds    | 598978395    |
| pankaj     | 10000012 | 2003 | nanakheda   | 37749986     |
| palak      | 10000012 | 2003 | tajplaca    | 795734987    |
| John       | 10000013 | 2004 | 123 Main St | 43893737     |
| riya       | 10000013 | 2004 | 282 street  | 77972987     |
| hrishika   | 10000013 | 2004 | tirupati    | 59597895     |
| aditya     | 10000013 | 2004 | diamonds    | 59897895     |
| aditi      | 10000013 | 2004 | diamonds    | 598978395    |
| pankaj     | 10000013 | 2004 | nanakheda   | 37749986     |
| palak      | 10000013 | 2004 | tajplaca    | 795734987    |
| John       | 10000014 | 2005 | 123 Main St | 43893737     |
| riya       | 10000014 | 2005 | 282 street  | 77972987     |
| hrishika   | 10000014 | 2005 | tirupati    | 59597895     |
| aditya     | 10000014 | 2005 | diamonds    | 59897895     |
| aditi      | 10000014 | 2005 | diamonds    | 598978395    |
| pankaj     | 10000014 | 2005 | nanakheda   | 37749986     |
| palak      | 10000014 | 2005 | tajplaca    | 795734987    |
| John       | 10000015 | 2006 | 123 Main St | 43893737     |
| riya       | 10000015 | 2006 | 282 street  | 77972987     |
| hrishika   | 10000015 | 2006 | tirupati    | 59597895     |
| aditya     | 10000015 | 2006 | diamonds    | 59897895     |
| aditi      | 10000015 | 2006 | diamonds    | 598978395    |
| pankaj     | 10000015 | 2006 | nanakheda   | 37749986     |
| palak      | 10000015 | 2006 | tajplaca    | 795734987    |
| John       | 10000016 | 2007 | 123 Main St | 43893737     |
| riya       | 10000016 | 2007 | 282 street  | 77972987     |
| hrishika   | 10000016 | 2007 | tirupati    | 59597895     |
| aditya     | 10000016 | 2007 | diamonds    | 59897895     |
| aditi      | 10000016 | 2007 | diamonds    | 598978395    |
| pankaj     | 10000016 | 2007 | nanakheda   | 37749986     |
| palak      | 10000016 | 2007 | tajplaca    | 795734987    |
| John       | 10000017 | NULL | 123 Main St | 43893737     |
| riya       | 10000017 | NULL | 282 street  | 77972987     |
| hrishika   | 10000017 | NULL | tirupati    | 59597895     |
| aditya     | 10000017 | NULL | diamonds    | 59897895     |
| aditi      | 10000017 | NULL | diamonds    | 598978395    |
| pankaj     | 10000017 | NULL | nanakheda   | 37749986     |
| palak      | 10000017 | NULL | tajplaca    | 795734987    |
+------------+----------+------+-------------+--------------+
56 rows in set (0.00 sec)

INNER JOIN

mysql> select c.cname,e.eid from course c  inner join enrollement e  on c.cid=e.cid;
+---------+----------+
| cname   | eid      |
+---------+----------+
| btech   | 10000010 |
| bsc     | 10000011 |
| mpharma | 10000012 |
| msc     | 10000013 |
| mca     | 10000014 |
| bca     | 10000015 |
+---------+----------+
6 rows in set (0.00 sec)

Hrishika verma CA 1 MITM, [7/14/2024 4:10 PM]
mysql> select c.cid,c.cname,e.eid from course c  inner join enrollement e  on c.cid=e.cid;
+------+---------+----------+
| cid  | cname   | eid      |
+------+---------+----------+
| 2001 | btech   | 10000010 |
| 2002 | bsc     | 10000011 |
| 2003 | mpharma | 10000012 |
| 2004 | msc     | 10000013 |
| 2005 | mca     | 10000014 |
| 2006 | bca     | 10000015 |

+------+---------+----------+
Now, we can write SQL queries to manage student records.

1. Insert a new student into the Students table:

INSERT INTO Students (student_id, first_name, last_name,
date_of_birth, address, phone_number) 
VALUES ('101', 'John', 'Doe', '1995/06/15', '123 Main St',
'5551234567');

2. Update the address of a specific student:

UPDATE Students 
SET address = '456 Elm St' 
WHERE student_id = '101';

3. Delete a specific student from the database:

DELETE FROM Students WHERE student_id = '101';

4. Retrieve all students who have enrolled in a particular course:

SELECT s.first_name, s.last_name 
FROM Students s 
JOIN Enrollments e ON s.student_id = e.student_id 
WHERE e.course_id = 'C001';

6 rows in set (0.00 sec)
