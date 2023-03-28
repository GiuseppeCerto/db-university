<!-- Group es. n. 1 -->

SELECT COUNT(*),YEAR(`students`.`enrolment_date`)
FROM `students`
GROUP BY YEAR(`students`.`enrolment_date`);

<!-- Group es. n. 2 -->

