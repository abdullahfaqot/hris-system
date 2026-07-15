# REST API Design

## Base URL

```
http://localhost:8000/api
```

---

# Authentication

| Method | Endpoint | Description |
|---------|----------|-------------|
| POST | /login | Login |
| POST | /logout | Logout |
| GET | /me | Current User |

---

# Department

| Method | Endpoint |
|---------|----------|
| GET | /departments |
| GET | /departments/{id} |
| POST | /departments |
| PUT | /departments/{id} |
| DELETE | /departments/{id} |

---

# Position

| Method | Endpoint |
|---------|----------|
| GET | /positions |
| GET | /positions/{id} |
| POST | /positions |
| PUT | /positions/{id} |
| DELETE | /positions/{id} |

---

# Employee

| Method | Endpoint |
|---------|----------|
| GET | /employees |
| GET | /employees/{id} |
| POST | /employees |
| PUT | /employees/{id} |
| DELETE | /employees/{id} |

---

# Payroll

| Method | Endpoint |
|---------|----------|
| GET | /payrolls |
| GET | /payrolls/{id} |
| POST | /payrolls |
| PUT | /payrolls/{id} |
| DELETE | /payrolls/{id} |

---

# Payslip

| Method | Endpoint |
|---------|----------|
| GET | /payslips |
| GET | /payslips/{id} |
| GET | /payslips/{id}/download |