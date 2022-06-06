## P5:
For the same table in P4, find how many bugs were created on "2019-03-01" or later. 
Your query should produce a table with one column called "count":
This problem is graded partially, 10% on correctness (your query gets the correct count) 
and 90% on performance (your query makes use of available indexes).

## My Solution:
SELECT count(created_at) AS count <br/>
FROM bugs<br/>
WHERE created_at >= '2019-03-01';

## Accepted Solution!!
## Score: 10% :(
