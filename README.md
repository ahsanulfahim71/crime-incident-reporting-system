# Crime Incident Report System

A web-based, database-driven application designed to digitally record, manage, and analyze crime-related incidents. Citizens can submit crime reports, while police authorities and administrators manage reports, stations, users, and analytics through role-based dashboards.

This project was developed as part of **CSE370: Database Systems**.

---

## 📌 Project Overview

The Crime Incident Report System modernizes crime data handling by replacing manual processes with a structured digital platform. The project emphasizes proper database design, normalization, and secure server-side processing using **PHP** and **MySQL**.

It demonstrates how a real-world database system can be integrated with a full-stack web application.

---

## 🛠️ Tech Stack

- **Frontend:** HTML, CSS  
- **Backend:** PHP  
- **Database:** MySQL  
- **Tools:** XAMPP, phpMyAdmin  
- **Version Control:** Git, GitHub  

---

## ✨ Core Features

### 👤 User Features
- Crime report submission  
- View personal report status  
- View police station details  

### 👮 Police Features
- Police station dashboard  
- View and manage assigned crime reports  
- Update crime report status  

### 🛡️ Admin Features
- Admin dashboard  
- Manage crime reports  
- Manage users (Admin and Police)  
- Manage police stations  
- View system-wide statistics and analytics  
- Role-based access control (RBAC)  

---

## 🔐 Authentication & Login System

The system implements a role-based authentication mechanism with separate login access for **Admin** and **Police** users.

### 🛡️ Admin Login
- Admin users log in using secure credentials.
- After login, admins are redirected to the **Admin Dashboard**.
- Admin users can:
  - Manage crime reports
  - Manage users and roles
  - Manage police stations
  - View analytics and system-wide statistics

### 👮 Police Login
- Police users log in using credentials created by the Admin.
- After login, police users are redirected to the **Police Dashboard**.
- Police users can:
  - View assigned crime reports
  - Update report status
  - Access police station-specific information

### 🔒 Access Control
- Role-based access control (RBAC) is enforced using PHP sessions.
- Unauthorized access to protected pages is restricted.
- Each dashboard and module is accessible only to authorized roles.

---

## 🔑 Demo Login Credentials (For Testing)

| Role   | Username | Password  |
|--------|----------|-----------|
| Admin  | admin    | admin123  |
| Police | police1  | police123 |

> ⚠️ These credentials are for demonstration and academic testing purposes only.

---

## 🧩 Database Design

- ER / EER Diagram  
- Relational Schema Diagram (phpMyAdmin style)  
- Fully normalized database schema:
  - First Normal Form (1NF)
  - Second Normal Form (2NF)
  - Third Normal Form (3NF)
- Optimized SQL queries for efficient data retrieval  

---

## 🖥️ Screenshots

Screenshots of the application are available in the `/screenshots` folder.

```
/screenshots
├── user-dashboard.png
├── police-dashboard.png
└── admin-dashboard.png
```

---

## 👥 Team Members & Contributions

### Ahsanul Fahim Ahmed
- Designed and implemented the core MySQL database schema and relationships  
- Developed the crime report submission and storage workflow  
- Implemented report status tracking and user-facing report views  
- Built police station information pages and police dashboard functionality  
- Implemented backend data handling using PHP and MySQL  

### Md Ashraful Hoque
- Designed and developed the administrative dashboard and workflows  
- Implemented admin-side crime report review and management features  
- Developed user and police station management modules  
- Built system-wide statistics and analytics for administrative insights  
- Implemented role-based access control (RBAC) and session-based authorization  
- Handled frontend styling and usability for administrative interfaces  

---

## ⚙️ How to Run Locally (XAMPP)

1. Install **XAMPP** and start **Apache** and **MySQL**.
2. Copy the project folder into:
   ```
   xampp/htdocs/Crime-Incident-Report-System
   ```
3. Open **phpMyAdmin** and create a database:
   ```
   crime_incident_db
   ```
4. Import the SQL file from the project (example):
   ```
   /database/crime_incident_db.sql
   ```
5. Update database configuration in the PHP config file (example):
   ```
   /config/db.php
   ```
   Set database host, username, password, and database name.
6. Open the application in your browser:
   ```
   http://localhost/Crime-Incident-Report-System/
   ```

---

## 📌 Notes

- This project is intended for academic and demonstration purposes.
- Do not commit real credentials or sensitive data.
- The system demonstrates core database concepts such as relational design, normalization, and role-based access control.

---
