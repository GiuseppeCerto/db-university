<!-- Join es. n. 1 -->

SELECT * FROM `degrees` 
JOIN `students`
ON `degrees`.`id`= `students`.`degree_id`
WHERE `degrees`.`name` = 'Corso di laurea in Economia';

<!-- Join es. n. 2 -->

SELECT * 
FROM `departments` 
JOIN `degrees`
ON `departments`.`id`= `degrees`.`department_id`
WHERE `departments`.`name` = 'Dipartimento di Neuroscienze' AND `degrees`.`level` = 'magistrale';

<!-- Join es. n. 3 -->

