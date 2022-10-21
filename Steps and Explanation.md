# SQL-Task-Edubridge

Scenario Based Questions - SQL_EduBridge

--Bahir KN --Create a Table for the Semester Examination Table the Required Attributes are Enrollment No, Student Name, Section, Subject Id, Marks.

 CREATE TABLE sem_examination (enrollment_no int PRIMARY KEY,
                      student_name varchar(20),                       
                      section varchar(5),                          
                      subject_id varchar(20),                          
                      marks int);
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
--To display the table with the above attribute values

SELECT * FROM sem_examination;
--To know the value which are all Greater Than or Equal to 75 marks

SELECT section , COUNT(section) AS NO_OF_CANDIDATE_greater_than_or_equal_to_75_marks
FROM sem_examination where marks>=75 group by section;
