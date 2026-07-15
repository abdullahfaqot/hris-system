# Deployment Guide

## Development

Requirements

- PHP 8.4
- Composer
- Node.js LTS
- PostgreSQL
- Docker

---

## Backend

```
cd backend

composer install

cp .env.example .env

php artisan key:generate

php artisan migrate

php artisan serve
```

---

## Frontend

```
cd frontend

npm install

npm run dev
```

---

## Production

```
php artisan config:cache

php artisan route:cache

php artisan optimize

npm run build
```