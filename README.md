# 🚌 BUSYS BUS Management System

> A comprehensive Bus Management and Reservation System for modern bus operations.

**BUSYS** is a full-stack web application that streamlines bus company operations — from route management and trip dispatching to seat reservations, payment verification, and fare calculation. Built with modern web technologies for real-world bus fleet management.

---

## 📋 Table of Contents

- [About](#-about)
- [Key Features](#-key-features)
- [Tech Stack](#️-tech-stack)
- [System Architecture](#️-system-architecture)
- [Seat Configuration](#-seat-configuration)
- [User Roles](#-user-roles)
- [Getting Started](#-getting-started)
- [Project Structure](#️-project-structure)
- [System Status](#-system-status)
- [Development Team](#-development-team)
- [License](#-license)

---

## 🎯 About

**BUSYS** handles the complete operations of a bus company, providing:

- 🗺️ **Route & Stop Management** — Define routes with multiple stops and distances
- 📅 **Trip Scheduling & Dispatching** — Schedule trips, assign buses, track departures
- 🪑 **Seat-Level Booking** — Real-time seat inventory with interactive seat maps
- 🚌 **Dynamic Seat Configuration** — Auto-adjusts per bus type and capacity
- 💰 **Fare Calculation** — LTFRB-compliant fare matrix with discounts
- 💳 **Payment Verification** — GCash, Bank Transfer, Cash workflows
- 🎫 **QR Code Ticketing** — HMAC-signed QR codes for secure boarding
- 🔐 **Role-Based Access Control** — 5 distinct user roles
- 🌐 **Multi-Language Support** — English + Tagalog
- 📊 **Audit Logging** — Complete system action tracking
- 📈 **Daily Sales Reports** — Real-time revenue analytics

Designed as a **Future Capstone Project** demonstrating real-world software engineering practices.

---

## ✨ Key Features

### 🚌 **Admin**

Complete management of bus operations and system configuration.

- **Bus Management**
  - Full CRUD for Buses, Routes, Trips, and Fares
  - Bus Name, Bus Number, Plate Number
  - Dynamic seat layout (2x2, 3x2, 2x1, 1x1)
  - Seat capacity with ±5 adjustment
  - Back row configuration
- **System Management**
  - User management (create, edit, suspend, delete)
  - Role-based access control
  - System audit logs viewer
  - Daily sales reports

### 📱 **Passenger**

Seamless booking experience for end-users.

- **Trip Discovery**
  - Browse and search available trips
  - Bus information display (number, name, type)
  - Fare calculator
- **Online Booking**
  - Real-time seat selection (interactive seat map)
  - Discount types: Student, Senior, PWD
  - Payment proof upload (GCash, Bank Transfer)
  - QR ticket generation
- **Booking Management**
  - View all bookings
  - Cancel bookings (with time-lock policy)
  - Booking confirmation page

### 💼 **Staff**

Day-to-day operations and customer service.

- **Booking Management**
  - View, confirm, and manage bookings
  - Cancel bookings with reason
  - Passenger manifest access
- **Payment Verification**
  - Review uploaded payment proofs
  - Approve / Reject payments
  - View daily sales overview
- **Walk-In Booking**
  - Create bookings for walk-in customers
  - Cash payment handling
  - Printable receipt
- **QR Verification**
  - Scan QR (camera / USB / upload image)
  - Manual booking reference lookup
  - Print professional boarding ticket

### 🎫 **Dispatcher**

Real-time trip operations and monitoring.

- **Trip Dispatch**
  - Real-time dispatch dashboard
  - Update trip status (scheduled → in_transit → completed)
  - Track actual departure/arrival times
- **Passenger Monitoring**
  - View passenger manifests per trip
  - Monitor trip progress

### 🌐 **Multi-Language**

- **English** and **Tagalog** support
- Auto-detection from browser
- Persistent user preference (localStorage)
- Role-aware translation (passenger pages translated; internal tools in English)

---

## 🏗️ Tech Stack

### **Frontend**

| Technology | Purpose |
|------------|---------|
| **React 18** | UI library |
| **Vite** | Build tool & dev server |
| **React Router v6** | Client-side routing |
| **Tailwind CSS** | Utility-first styling |
| **Axios** | HTTP client |
| **React Hot Toast** | Toast notifications |
| **Lucide React** | Icon library |
| **i18next** | Internationalization |
| **html5-qrcode** | QR scanning (camera + upload) |
| **qrcode.react** | QR code generation |

### **Backend**

| Technology | Purpose |
|------------|---------|
| **FastAPI** | Python web framework |
| **SQLAlchemy** | ORM |
| **MySQL** | Relational database |
| **Alembic** | Database migrations |
| **Pydantic** | Data validation |
| **python-jose** | JWT authentication |
| **Passlib + Bcrypt** | Password hashing |
| **SlowAPI** | Rate limiting |
| **APScheduler** | Background jobs |
| **HMAC-SHA256** | QR signature |

### **DevOps & Tools**

| Technology | Purpose |
|------------|---------|
| **Git & GitHub** | Version control |
| **Uvicorn** | ASGI server |
| **npm** | Package manager |

---

## 🏛️ System Architecture
