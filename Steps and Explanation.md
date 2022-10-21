# SQL-Task-Edubridge

Scenario Based Questions - SQL_EduBridge

--NambiRajan K --Create a Table for the Semester Examination Table the Required Attributes are Enrollment No, Student Name, Section, Subject Id, Marks.


CREATE TABLE class_data (enrollment_no varchar(10), student_name varchar(10), class_section varchar(10),subject_id varchar(10),marks INT, primary key (enrollment_no));

--Inserting values as required for the above attributes

INSERT INTO  sem_examination VALUES(1, 'Tim', 'A',1,70);
INSERT INTO  sem_examination VALUES(2, 'Jim', 'A',2,75);
INSERT INTO  sem_examination VALUES(3, 'Kim', 'B',3,65);
INSERT INTO  sem_examination VALUES(4, 'Tom', 'B',4,77);
INSERT INTO  sem_examination VALUES(5, 'John','C',5,60);
INSERT INTO  sem_examination VALUES(6, 'Joe', 'C',1,82);
INSERT INTO  sem_examination VALUES(7, 'James', 'B',2,76);
INSERT INTO  sem_examination VALUES(8, 'Henry', 'C',5,68);
INSERT INTO  Sem_examination VALUES(9, 'Matt', 'B',3,71);
INSERT INTO  sem_examination VALUES(10, 'Paul', 'A',4,79);

--To know the value which are all Greater Than or Equal to 75 marks


SELECT class_section,COUNT(enrollment_no) AS NO_OF_CANDIDATE FROM class_data WHERE MARKS>=75 GROUP BY class_section;
