# Домашнее задание к занятию "`12.1. RDB`" - `Белов Максим`


### Задание 1

employee (
- id_employee, primary key, serial,
- last_name, varchar(50),
- first_name, varchar(50),
- patronymic, varchar(50),
- hire_date, date
- salary, real
- id_position, foreign key, integer
- id_structural_division, foreign key, integer
- id_branch_office, foreign key, integer  
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
- id_region, foreign key, integer,
- id_city, foreign key, integer,
- branch_office_address, varchar(500)  
)

region (
- id_region,  primary key, serial,
- region_name, varchar(100)  
)

city (
- id_city, primary key, serial,
- id_region, primary key, integer,
- city_name, varchar(50)  
)

project (
- id_project, primary key, serial
- project_name, varchar(100)  
)

project_employee (
- id_project, foreign key, integer
- id_employee, foreign key, integer  
)
