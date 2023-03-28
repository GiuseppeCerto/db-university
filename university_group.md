<!-- Group es. n. 1 -->

SELECT COUNT(*),YEAR(`students`.`enrolment_date`)
FROM `students`
GROUP BY YEAR(`students`.`enrolment_date`);

<!-- Group es. n. 2 -->

SELECT `teachers`.`office_address`, COUNT(*)
FROM `teachers`
GROUP BY `teachers`.`office_address`;

<!-- Group es. n. 3 -->

SELECT `exam_student`.`exam_id`, AVG(`exam_student`.`vote`)
FROM `exam_student`
GROUP BY `exam_student`.`exam_id`;

<!-- Group es. n. 4 -->

SELECT `degrees`.`department_id`, COUNT(*)
FROM `degrees`
GROUP BY `degrees`.`department_id`;
