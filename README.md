# Trading Journal

**Status:** 🚧 In Development

Trading Journal is a full-stack application built with **Laravel 12 (API-only)** and **Vue.js 3**. It is designed to help users track and manage their trading activity.

> ⚠️ **This project is currently under development and primarily serves as a portfolio piece to showcase my skills as a developer.**

---

## 🧱 Tech Stack

- **Laravel 12** (REST API)
- **Laravel Sanctum** (API token auth)
- **Vue.js 3** (frontend SPA)
- **MySQL / MariaDB**
- **Vite** (frontend dev server)
- **Axios** (for HTTP requests)

---

## ⚙️ Backend Setup (Laravel)

cd trading-journal

# Install dependencies
composer install

# Copy .env and configure
cp .env.example .env

# Generate app key
php artisan key:generate

# Configure your DB in .env
DB_DATABASE=trading_journal
DB_USERNAME=root
DB_PASSWORD=

# Run migrations
php artisan migrate

# Run the application
php artisan serve

---

## ⚙️ FrontEnd Setup (Vue)

cd frontend

# Install dependencies
npm install

# Start dev server
npm run dev
