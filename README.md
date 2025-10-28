# 📚 Library Management System

A **Laravel-based CRUD MVC Web Application** designed to manage library resources such as books, members, and borrow/return transactions efficiently.  
This project was developed as part of the **Midterm Examination** for the IT course on SYSTEM INTEGRATION.

---


---

## 🧾 Overview
The **Library Management System** allows administrators and librarians to **create, read, update, and delete (CRUD)** book records, manage users, and track borrowing and returning activities.  
It follows the **Model-View-Controller (MVC)** design pattern for better structure and maintainability.

---

## ⚙️ Features
✅ Add, edit, delete, and view book information  
✅ Manage member records (students, teachers, etc.)  
✅ Record and track book borrowing and returning  
✅ Search and filter books  
✅ Responsive user interface using Blade templates  
✅ Database migration and seeding  
✅ Validation and authentication (Laravel Breeze or default Auth)

---

## 🏗️ System Design (MVC)

### **Model (M)**
Handles data and database logic using Eloquent ORM.  
Example Models:
- `Book.php`
- `Member.php`
- `BorrowRecord.php`

### **View (V)**
Manages the presentation layer using **Blade templates**.  
Example Views:
- `resources/views/books/index.blade.php`
- `resources/views/books/edit.blade.php`

### **Controller (C)**
Contains logic that connects the model and view.  
Example Controllers:
- `BookController.php`
- `MemberController.php`
- `BorrowController.php`

---

## 🧮 CRUD Operations

| Operation | HTTP Method | Description | Example Route |
|------------|-------------|--------------|----------------|
| **Create** | POST | Add a new book | `/books` |
| **Read** | GET | Display book list | `/books` |
| **Update** | PUT/PATCH | Edit book details | `/books/{id}` |
| **Delete** | DELETE | Remove a book | `/books/{id}` |

---

## 🖥️ Installation Guide

1. **Clone the repository**
   ```bash
   git clone https://github.com/<your-username>/library-management-system.git
   cd library-management-system
2. Install Dependencies
composer install
npm install
3.Create Environment File
cp .env.example .env
4.Generate application key
php artisan key:generate
5.Set up database connection
 *Open .env and update:
DB_DATABASE=library_db
DB_USERNAME=root
DB_PASSWORD=

6.Run Migration Seeders
php artisan migrate --seed

7. Start development server
   php artisan serve

8. Access the app
   Open in browser: http://localhost:8000
  8000

🗄️ Database Structure
Tables:
books – stores book details
members – stores member information
borrow_records – stores borrowing and returning transactions
users – stores authentication data (if login is implemented)

![Dashboard Screenshot](screenshots/dashboard.png)
![Book List](screenshots/book-list.png)

GitHub

👨‍💻 Developer Information

Name: Marian Vallo
Course/Section: BSIT – 4B
Date: October 2025
Project: Midterm Examination – Laravel CRUD MVC System

📝 This Library Management System is developed for educational purposes as part of the Midterm Examination in Web Application Development.
