# Business Requirement Document (BRD)

# Human Resource Information System (HRIS)

Version : 1.0.0

Author : Abdullah Faqot

Last Update : July 2026

---

# 1. Introduction

## 1.1 Background

Human Resource Information System (HRIS) adalah aplikasi berbasis web yang digunakan untuk membantu perusahaan dalam mengelola data karyawan, struktur organisasi, proses payroll, dan pembuatan slip gaji secara digital.

Pada banyak perusahaan kecil hingga menengah, proses administrasi karyawan masih dilakukan menggunakan Microsoft Excel sehingga sering terjadi kesalahan perhitungan, duplikasi data, dan kesulitan dalam pelaporan. Oleh karena itu dibutuhkan sistem yang terintegrasi untuk meningkatkan efisiensi operasional.

---

## 1.2 Objective

Project ini bertujuan untuk:

- Mengelola data karyawan secara terpusat.
- Mengelola departemen dan jabatan.
- Mengotomatisasi proses payroll.
- Menghasilkan slip gaji dalam format PDF.
- Menyediakan dashboard informasi HR.

---

## 1.3 Project Scope

### In Scope

- Authentication
- Authorization
- Dashboard
- Employee Management
- Department Management
- Position Management
- Payroll Management
- Payslip PDF
- User Management

### Out of Scope

Untuk versi 1.0 fitur berikut belum dikembangkan:

- Attendance
- Leave Management
- Overtime
- Recruitment
- Performance Appraisal
- Asset Management
- BPJS Calculation
- Tax (PPh21)

---

# 2. Stakeholders

| Role | Responsibility |
|------|----------------|
| Administrator | Mengelola seluruh sistem |
| HR Staff | Mengelola data karyawan |
| Payroll Staff | Mengelola payroll |
| Employee | Melihat profil dan slip gaji |

---

# 3. Functional Requirements

## Authentication

- Login
- Logout
- Change Password

---

## Dashboard

Menampilkan:

- Total Employee
- Total Department
- Total Position
- Total Payroll Bulan Ini

---

## Department

- Create Department
- Update Department
- Delete Department
- View Department

---

## Position

- Create Position
- Update Position
- Delete Position
- View Position

---

## Employee

- Create Employee
- Update Employee
- Delete Employee
- View Employee
- Search Employee
- Pagination

---

## Payroll

- Generate Payroll
- Payroll History
- Payroll Detail

---

## Payslip

- Generate PDF
- Download PDF

---

# 4. Non Functional Requirements

## Performance

Response API maksimal 3 detik.

---

## Security

- Password Hashing
- Laravel Sanctum Authentication
- Role & Permission
- Input Validation

---

## Availability

Aplikasi dapat diakses melalui browser modern.

---

## Browser Support

- Google Chrome
- Microsoft Edge
- Mozilla Firefox

---

# 5. Technology Stack

## Backend

- Laravel 12
- PHP 8.4

## Frontend

- React
- TypeScript
- Vite
- Tailwind CSS
- shadcn/ui

## Database

- PostgreSQL

## Others

- Docker
- Git
- GitHub

---

# 6. Success Criteria

Project dianggap berhasil apabila:

- User dapat login.
- CRUD Department berjalan.
- CRUD Position berjalan.
- CRUD Employee berjalan.
- Payroll berhasil dibuat.
- Slip gaji dapat diunduh.
- Dashboard menampilkan statistik.

---

# 7. Future Enhancement

Fitur yang akan dikembangkan pada versi berikutnya:

- Attendance Management
- Leave Management
- Overtime
- BPJS
- Tax Calculation
- Email Payslip
- Notification
- Audit Log
- Multi Company