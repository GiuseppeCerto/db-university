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

<!-- SOLUZIONE TROVATA SU INTERNET (chiedere come funzionano le funzioni) -->

<!-- es. n. 4 -->

SELECT *
FROM `courses`
WHERE `period` = 'I semestre' AND `year` = 1;

<!-- es. n. 5 -->

SELECT *
FROM `exams`
WHERE `date` = `2020-06-20` AND `hour` > `14:00:00`;

<!-- es. n. 6 -->

SELECT *
FROM `degrees`
WHERE `level` = 'magistrale';

<!-- es. n. 7 -->

SELECT count(*)
FROM `departments`;

<!-- es. n. 8 -->

SELECT *
FROM `teachers`
WHERE `phone` IS NULL;