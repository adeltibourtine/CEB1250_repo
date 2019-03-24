# CEB1250_repo
CEB1250_repo

CREATE TABLE course (
course_id INTEGER PRIMARY KEY,
course_name VARCHAR(50) not null,
course_description VARCHAR(100) not null
)

alter table course add course_day VARCHAR(50) not null

Get all female employees

SELECT *
FROM employees
WHERE gender = ÔFÕ;

Get all employees hired after 01-01-1995

SELECT *
FROM employees
WHERE hire_date > '1995-01-01Õ;

Get all the valid titles (with to_date equals to 01-01-9999)

SELECT *
FROM titles
WHERE to_date = '9999-01-01';

SELECT DISTINCT title
FROM titles
WHERE to_date = '9999-01-01';

Get all salaries from 60000 to 90000

SELECT *
FROM salaries
WHERE salary
BETWEEN 60000 AND 90000;

Get all titles where title is equal to engineer

SELECT *
FROM titles
WHERE title = 'Engineer';

Insert a new row into course table with 1, ÔCED-1250Õ, ÔBig Data StorageÕ

INSERT INTO course (course_id, course_name, course_description)
VALUES (1, 'CEBD-1250', 'Big Data Storage');

Delete all male employees hired at 01-01-2009

DELETE FROM employees
WHERE gender = 'M'
AND hire_date = '2009-01-01';

Update the salary of employee 499984 to 100000

UPDATE salaries
SET salary = 100000
WHERE emp_no = 499984
AND to_date = '9999-01-01';

Delete all titles not valid (with to_date not equal to 01-01-9999)

SELECT *
FROM titles
WHERE to_date <> '9999-01-01';



Get all female employees
Get all employees hired after 01-01-1995
Get all the valid titles (with to_date equals to 01-01-9999)
Get all salaries from 60000 to 90000
Get all titles where title is equal to engineer
Insert a new row into course table with 1, ÔCED-1250Õ, ÔBig Data StorageÕ
Delete all male employees hired at 01-01-2009
Update the salary of employee 499984 to 100000
Delete all titles not valid (with to_date not equal to 01-01-9999)
