# Домашнее задание к занятию "`12.1. RDB`" - `Белов Максим`


### Задание 1

employee (
- id_employee, primary key, serial,
- last_name, varchar(50)
- id_first_name, foreign key, integer
- id_patronymic, foreign key, integer
- hire_date, date
- salary, real
- id_position, foreign key, integer
- id_structural_division, foreign key, integer
- id_branch_office, foreign key, integer  
)

first_name (
- id_first_name, primary key, serial,
- name, varchar(50)  
)

patronymic (
- id_patronymic, primary key, serial,
- patronymic_name, varchar(50)  
)

position (
- id_position, primary key, serial,
- -position_name, varchar(100)  
)

structural_division (
- id_structural_division, primary key, serial,
- id_division_type, primary key, integer,
- structural_division_name, varchar(500)  
)

division_type (
- id_division_type, primary key, serial,
- division_type_name, varchar(50)  
)

branch_office (
- id_branch_office, primary key, serial,
- branch_office_address, varchar(max)  
)

project (
- id_project, primary key, serial
- project_name, varchar(100)  
)

project_employee (
- id_project, foreign key, integer
- id_employee, foreign key, integer  
)
