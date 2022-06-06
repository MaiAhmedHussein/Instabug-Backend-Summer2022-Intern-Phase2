## P1:
Given 3 tables, students(id, name) , courses(id, name) , grades(id, course_id, student_id, grade), find the top 100 students based on their
average grades sorted descendingly by the average grade and in case multiple students have the same average grade, sort them lexicographically in ascending order by their names.
Your query should output a table with the following columns (name, average_grade):

## My Answer:

SELECT students.name AS name,  AVG(grade)  AS average_grade <br/>
FROM grades <br/>
JOIN students ON students.id = student_id<br/>
GROUP BY student_id , students.name<br/>
ORDER BY AVG(grade) DESC, students.name<br/>
LIMIT 100;

## Accepted Solution !!
## Score: 100%
