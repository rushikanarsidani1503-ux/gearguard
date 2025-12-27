# ⚙️ GearGuard – The Ultimate Maintenance Tracker

GearGuard is a role-based **Maintenance Management System** designed to help organizations track equipment, manage maintenance teams, and handle corrective and preventive maintenance efficiently using an ERP-style workflow.

## 📌 Problem Statement

Companies face challenges in:
- Tracking equipment and ownership
- Managing breakdowns and routine maintenance
- Assigning technicians and responsibilities
- Monitoring repair status and asset lifecycle

**GearGuard solves this by seamlessly connecting:**
- 🏭 Equipment (what is broken)
- 👥 Teams (who fix it)
- 🛠️ Requests (the work to be done)

## 🚀 Key Features

### 🔐 Login & Role-Based Access
- **User**: Create maintenance requests
- **Technician**: Update request status
- **Manager**: Assign, schedule, and scrap equipment

### 🏭 Equipment Management
- Track equipment by department or employee
- Store serial number, warranty, and location
- Assign default technician
- Automatic scrap flag when equipment is unusable

### 🛠️ Maintenance Requests
- **Corrective Maintenance** (breakdowns)
- **Preventive Maintenance** (scheduled)
- Auto-assignment of technician from equipment
- Lifecycle stages:
  - New
  - In Progress
  - Repaired
  - Scrap


### 📋 Smart Automation
- Auto-fill team & technician
- Overdue request detection
- Scrap logic automatically updates equipment status
- Kanban workflow for technicians

### 📊 Dashboard
- Total equipment
- Total maintenance requests
- Open requests count

## 🖥️ User Interface

### Kanban Board
- Grouped by maintenance stages
- Click-to-update workflow
- Visual overdue indicators

### Dashboard
- Management overview of system health

## 🧱 Tech Stack

| Layer | Technology |
|------|-----------|
| Backend | PHP |
| Database | MySQL |
| Frontend | HTML, CSS, JavaScript |
| Server | Apache (XAMPP) |

## 📁 Project Structure
gearguard/
│
├── login.php
├── logout.php
├── index.php
├── dashboard.php
├── style.css
├── script.js
│
├── api/
│ ├── db.php
│ └── requests.php
│
└── database/
└── gearguard.sql

## ⚙️ Installation & Setup

### 1️⃣ Prerequisites
- XAMPP / WAMP
- PHP 8+
- MySQL


### 2️⃣ Steps to Run

1. Copy project folder to:
   xampp/htdocs/gearguard
2. Start **Apache** and **MySQL** from XAMPP
3. Open phpMyAdmin:
   http://localhost/phpmyadmin
4. Create database:
   gearguard
5. Import:
   database/gearguard.sql
6. Open browser:
   http://localhost/gearguard/login.php
