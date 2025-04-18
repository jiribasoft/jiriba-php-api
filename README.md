# 🚀 Jiriba PHP API Framework

**A lightweight, modular PHP API framework built by Jiribasoft for rapid backend development with clean architecture and simplicity.**

---

## 🧠 Overview

The **Jiriba PHP API Framework** is a custom-built micro-framework that helps you:

- 🎯 Quickly scaffold API projects
- 🧩 Modularize your controllers and routes
- 🗄️ Connect to and auto-create MySQL tables based on your configuration
- 📦 Handle backups, logging, request metadata, and admin setup with ease
- 🛠️ Customize everything — but keep it simple

---

## ⚙️ Configuration

All configuration is handled via `src/Config.php`.

You define:

- 📌 Database credentials
- 🧱 Table structures
- 📂 Upload folders
- 🔐 Admin role and permissions
- 🌍 Global constants

---

## 💾 Database Initialization

Tables are auto-created based on `Config::TABLES` using:

```php
$model = new Model();
$model->init();
