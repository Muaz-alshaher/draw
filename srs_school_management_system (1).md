# 📄 Software Requirements Specification (SRS)

## School Management System (SMS)

### Version 1.0.0 (Revised - IEEE 830 Aligned)

---

## 1. Introduction

### 1.1 Purpose

This document defines the functional and non-functional requirements for the School Management System (SMS). It serves as a contract between stakeholders and the development team. The system will be implemented using Laravel (Backend) and Flutter (Frontend).

### 1.2 Intended Audience

- Developers (Backend & Frontend)
- System Architects
- QA/Test Engineers
- Project Managers

### 1.3 Product Scope

SMS is a multi-application platform to manage school operations including users, attendance, schedules, assessments, invoices, and notifications across four roles: Admin, Teacher, Student, Parent.

### 1.4 Definitions

- SRS: Software Requirements Specification
- API: Application Programming Interface
- JWT: JSON Web Token

### 1.5 References

- IEEE 830-1998
- Laravel Documentation
- Flutter Documentation

---

## 2. Overall Description

### 2.1 Product Perspective

System follows Clean Architecture and API-First design. Backend exposes RESTful APIs consumed by Flutter apps.

### 2.2 Product Functions (High-Level)

- User Management
- Attendance Management
- Schedule Management
- Assessment & Marks
- Invoice & Payment System
- Notification System
- File Management

### 2.3 User Classes

| User | Description |
|------|------------|
| Admin | Full control |
| Teacher | Manage classes, attendance, marks |
| Student | View schedule, marks |
| Parent | Monitor student & payments |

### 2.4 Operating Environment

- Backend: Laravel (PHP)
- Frontend: Flutter (Android)
- Database: MySQL
- Server: Linux / Cloud Hosting

### 2.5 Constraints

- Must use Laravel
- Must follow Clean Architecture
- Mobile-first approach

### 2.6 Assumptions

- Internet connection available
- Users have smartphones

---

## 3. External Interfaces

### 3.1 User Interface

- Mobile UI for all roles except Admin (optional web)

### 3.2 Hardware

- Mobile devices (Android)

### 3.3 Software

- REST API
- Firebase Notifications

### 3.4 Communication

- HTTPS + JSON

---

## 4. System Features

### 4.1 User Management

- FR-1: System shall create user accounts
- FR-2: System shall retrieve user accounts
- FR-3: System shall delete user accounts
- FR-4: System shall authenticate users
- FR-5: System shall assign roles
- FR-6: System shall display user profile
- FR-7: System shall update user profile

### 4.2 Attendance System

- FR-8: System shall record attendance
- FR-9: System shall send notification to parents
- FR-10: System shall generate attendance reports

### 4.3 Notification System

- FR-11: System shall send broadcast notifications
- FR-12: System shall send targeted notifications

### 4.4 Schedule Management

- FR-13: System shall create schedules
- FR-14: System shall update schedules
- FR-15: System shall delete schedules
- FR-16: System shall assign teacher & subject
- FR-17: System shall display schedules

### 4.5 Material Management

- FR-18: System shall manage materials
- FR-19: System shall assign materials to classes
- FR-20: System shall upload books

### 4.6 File Management

- FR-21: System shall upload files
- FR-22: System shall download files

### 4.7 Payment System

- FR-23: System shall generate invoices
- FR-24: System shall record payments
- FR-25: System shall display invoices
- FR-26: System shall notify overdue payments

### 4.8 Student Marks

- FR-27: System shall display marks
- FR-28: System shall generate reports

### 4.9 Assessment Management

- FR-29: System shall manage assessments
- FR-30: System shall assign marks

---

## 5. Non-Functional Requirements

### 5.1 Performance

- API response < 500ms

### 5.2 Security

- JWT Authentication
- Role-based access control
- Password hashing

### 5.3 Scalability

- Redis caching & queues

### 5.4 Availability

- Uptime ≥ 99%

### 5.5 Maintainability

- Layered architecture (Clean Architecture)

---

## 6. Other Requirements

### 6.1 Database

- Relational DB
- Transactions support

### 6.2 Logging

- Error logging
- Monitoring system

---

## 7. Appendices

- ERD
- API Documentation (Postman )

---

## ✅ Approval

This document must be approved before development phase.
