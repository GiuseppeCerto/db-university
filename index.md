<!-- es. n. 1 -->

SELECT *
FROM `students`
WHERE YEAR(date_of_birth) = 1990;

<!-- es. n. 2 -->

SELECT *
FROM `courses`
WHERE `cfu` > 10;

<!-- es. n. 3 -->

SELECT * 
FROM students 
WHERE date_of_birth <= DATE_SUB(CURDATE(), INTERVAL 30 YEAR);

<!-- es. n. 4 -->

SELECT *
FROM `courses`
WHERE `period` = 'I semestre' AND `year` = 1;