# Database Design

## Database

PostgreSQL

---

## Tables

### users

Laravel Authentication.

---

### departments

Master Department.

| Column | Type |
|---------|------|
| id | bigint |
| code | varchar(20) |
| name | varchar(100) |
| description | text |

---

### positions

| Column | Type |
|---------|------|
| id | bigint |
| department_id | bigint |
| code | varchar(20) |
| name | varchar(100) |

---

### employees

| Column | Type |
|---------|------|
| id | bigint |
| user_id | bigint |
| department_id | bigint |
| position_id | bigint |
| employee_code | varchar(20) |
| nik | varchar(20) |
| fullname | varchar(150) |
| gender | enum |
| birth_date | date |
| phone | varchar(20) |
| email | varchar(100) |
| address | text |
| hire_date | date |
| employment_status | enum |
| basic_salary | decimal |

---

### payrolls

| Column | Type |
|---------|------|
| id | bigint |
| employee_id | bigint |
| payroll_month | integer |
| payroll_year | integer |
| basic_salary | decimal |
| total_allowance | decimal |
| total_deduction | decimal |
| net_salary | decimal |
| generated_at | timestamp |

---

### payroll_details

| Column | Type |
|---------|------|
| id | bigint |
| payroll_id | bigint |
| component_name | varchar |
| component_type | enum |
| amount | decimal |

---

### payslips

| Column | Type |
|---------|------|
| id | bigint |
| payroll_id | bigint |
| file_path | varchar |
| generated_at | timestamp |

---

## Relationship

Department

1 ---- * Position

Department

1 ---- * Employee

Position

1 ---- * Employee

Employee

1 ---- * Payroll

Payroll

1 ---- * Payroll Detail

Payroll

1 ---- 1 Payslip