# SQL-Task-Edubridge

Scenario Based Questions - SQL_EduBridge

--NambiRajan K --Create a Table for the Semester Examination Table the Required Attributes are Enrollment No, Student Name, Section, Subject Id, Marks.


CREATE TABLE class_data (enrollment_no varchar(10), student_name varchar(10), class_section varchar(10),subject_id varchar(10),marks INT, primary key (enrollment_no));

--Inserting values as required for the above attributes

insert into  class_data values(1,'TIM','A',1,70);
insert into  class_data values(2,'JIM','A',2,75);
insert into  class_data values(3,'Kim','B',3,65);
insert into  class_data values(4,'TOM','B',4,77);
insert into  class_data values(5,'JOHN','C',5,60);
insert into  class_data values(6,'JOE','C',1,82);		
insert into  class_data values(7,'JAMES','B',2,76);
insert into  class_data values(8,'HENRY','C',5,68);
insert into  class_data values(9,'MATT','B',3,71);
insert into  class_data values(10,'PAUL','A',4,79);

--To know the value which are all Greater Than or Equal to 75 marks


SELECT class_section,COUNT(enrollment_no) AS NO_OF_CANDIDATE FROM class_data WHERE MARKS>=75 GROUP BY class_section;
