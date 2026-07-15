# Git Workflow

Branch Strategy

```
main
│
develop
│
feature/*
```

---

Main

Production Ready

---

Develop

Integration Branch

---

Feature

```
feature/authentication

feature/employee

feature/payroll

feature/dashboard
```

---

Workflow

```
git checkout develop

git checkout -b feature/employee

Coding

git add .

git commit -m "feat: employee CRUD"

git push

Pull Request

Merge ke develop
```