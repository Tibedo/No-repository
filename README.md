1) select first_name, last_name from employees;

2) select * from employees group by first_name;

3) select total(salary) from employees;

4) select min(salary), max(salary) from employees;

5) select first_name, salary/12.2 from employees;

6) select first_name, last_name, salary from employees where salary < 10000 and salary > 15000;

* 7) select first_name, last_name, salary from employees where salary < 10000 and salary > 15000 in (select department_id from departments where department_id = 30 or department_id = 100);

8) select last_name from employees where substr(last_name, 3) = 'e';

9) select job_id from employees;

10) select department_id, total(salary) from employees group by department_id;

11) select job_id, avg(salary) from employees where(job_id != 'IT_PROG') group by job_id;

* 12) select department_id, avg(salary) from employees where(employee_id > 10) group by department_id;

13) select first_name, last_name, salary from employees where salary > (select salary from employees where(last_name = 'Bull'));

* 14) select first_name, last_name from employees where(select country_id from locations where(country_id = 'US'));



