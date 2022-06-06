## P2:
For the same tables in P1, for each student, get all the courses that he/she is enrolled in along with the grade he/she scored for each course. 
Order the result by the student name in ascending order and if there is a tie, break it with the course name in ascending order and if there is a tie break it with the grade in ascending order. 
The final result should have 3 columns with names (name, course, grade):

## My Answer:

SELECT students.name AS name, courses.name AS course, grade AS grade <br/>
FROM grades, courses, students<br/>
where courses.id = course_id and students.id = student_id<br/>
GROUP BY student_id , students.name and course_id, courses.name,grade<br/>
ORDER BY students.name, courses.name, grade;

## Accepted Solution:
## Score: 100%
