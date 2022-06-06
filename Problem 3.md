## P3:
For the same tables in P1, get the name of the most popular course (the one where the most students are enrolled) 
and if there is a tie, get the course that's lexicographically the smallest:


## My Answer:
SELECT courses.name AS name<br/>
FROM grades <br/>
JOIN courses ON courses.id = course_id<br/>
GROUP BY course_id , courses.name<br/>
ORDER BY count(course_id) DESC, courses.name<br/>
LIMIT 1;

## Accepted Solution!!
## Score: 100%
