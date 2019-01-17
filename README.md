# JDBC_Assignment3

SQL: 3a

SHOW CREATE TABLE `sqlandjava`.`owners`;

SHOW CREATE TABLE `sqlandjava`.`owners`;
SELECT * FROM `sqlandjava`.`owners` LIMIT 1000;
SHOW CREATE TABLE `sqlandjava`.`owners`;
INSERT INTO `sqlandjava`.`owners` (`owner_id`, `person_id`, `car_id`) VALUES ('1', '2', '3');
SELECT `owner_id`, `person_id`, `car_id` FROM `sqlandjava`.`owners` WHERE  `owner_id`=1;
INSERT INTO `sqlandjava`.`owners` (`owner_id`, `person_id`, `car_id`) VALUES ('2', '1', '4');
SELECT `owner_id`, `person_id`, `car_id` FROM `sqlandjava`.`owners` WHERE  `owner_id`=2;
INSERT INTO `sqlandjava`.`owners` (`owner_id`, `person_id`, `car_id`) VALUES ('3', '3', '2');
SELECT `owner_id`, `person_id`, `car_id` FROM `sqlandjava`.`owners` WHERE  `owner_id`=3;
INSERT INTO `sqlandjava`.`owners` (`owner_id`, `person_id`, `car_id`) VALUES ('4', '4', '1');
SELECT `owner_id`, `person_id`, `car_id` FROM `sqlandjava`.`owners` WHERE  `owner_id`=4;


CREATE USER user@localhost IDENTIFIED BY 'password';
GRANT SELECT ON sqlandjava.owners TO user@localhost;
