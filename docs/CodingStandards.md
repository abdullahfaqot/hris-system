# Coding Standards

# Backend (Laravel)

## Naming Convention

Class

```
EmployeeController
PayrollService
DepartmentRepository
```

Method

```
getEmployees()
createEmployee()
generatePayroll()
```

Variable

```php
$employee
$basicSalary
$totalAllowance
```

Database Table

```
employees
departments
payroll_details
```

Column

```
employee_code
basic_salary
created_at
```

---

## Folder Structure

```
app/

Controllers/

Services/

Repositories/

Models/

Requests/

Policies/

Traits/

Enums/
```

---

## API Response

Success

```json
{
    "success": true,
    "message": "Employee created successfully",
    "data": {}
}
```

Error

```json
{
    "success": false,
    "message": "Validation Error",
    "errors": {}
}
```

---

# Frontend

Component

```
EmployeeTable.tsx
EmployeeForm.tsx
```

Hook

```
useEmployee.ts
```

API

```
employeeService.ts
```

Type

```
Employee.ts
```

Page

```
EmployeePage.tsx
```

---

# Git Commit Convention

```
feat:
fix:
refactor:
docs:
style:
test:
chore:
```

Example

```
feat: add employee CRUD
docs: update API documentation
fix: payroll calculation
```