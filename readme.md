# A Relational database Model Illustration

This repository contains an image file that illustrates a relational Database model with object, entities and relationships

The sample model entails a typical University with a Faculty has Dean, Hod, Lecturers, Undergraduates and Postgraduates

The following queries would relate to the relationship between the entities:

Sample Insert Query: INSERT into undergrad_students (undergrad_student_id, undergrad_student_name, undergrad_student_matric_number, undergrad_student_dept, undergrad_student_course, undergrad_student_faculty) VALUES (1,
'Jacky',011321,'English Department', 'General Studies' ,'Arts');

Sample Select Query: SELECT FROM postgrad_students WHERE undergrad_student_name LIKE '%Joy';

Sample Count Query: SELECT COUNT(hod_name) FROM hod_dept;

Sample Inner Join Query:  SELECT dean.dean_id, undergrad_student.undergrad_student_name, dean.dean_course, FROM dean INNER JOIN undergrad_student ON dean.dean_id=undergrad_student.undergrad_student_id;

Sample Update Query: UPDATE lecturer SET name='Adegbola', course='General Studies', WHERE name='Adegola';