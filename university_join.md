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

SELECT COUNT(`courses`.`name`) 
FROM `teachers` 
JOIN `course_teacher`
ON `teachers`.`id` = `course_teacher`.`teacher_id`
JOIN `courses`
ON `courses`.`id` = `course_teacher`.`course_id`
WHERE `teachers`.`name` = 'Fulvio' AND `teacher`.`surname` = 'Amato';

<!-- Join esw. n. 4 -->

SELECT `students`.`name`, `students`.`surname`, `degrees`.`name`, `courses`.`name`
FROM `students` 
JOIN `degrees`
ON `degrees`.`id` = `students`.`degree_id`
JOIN `courses`
ON `degrees`.`id` = `courses`.`degree_id`
ORDER BY `students`.`name` ASC;

<!-- Join es. n. 5 -->

SELECT `degrees`.`name`,`courses`.`name`,`teachers`.`name`,`teachers`.`surname`
FROM `degrees` 
JOIN `courses`
ON `degrees`.`id` = `courses`.`degree_id`
JOIN `course_teacher`
ON `degrees`.`id` = `course_teacher`.`course_id`
JOIN `teachers`
ON `teachers`.`id` = `course_teacher`.`course_id`;

<!-- Join es. n. 6 -->

