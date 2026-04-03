# 📄 Software Requirements Specification (SRS)

## School Management System

### version 1.0.0 approved

#### (IEEE 830 Compliant)

---

## 1. Introduction

### 1.1 Purpose

This document provides a detailed description of the requirements for the School Management System (SMS). It is intended for stakeholders including developers, system architects, testers, and project managers. The system will be implemented using Laravel (Backend) and Flutter (Frontend).

### 1.2 Scope

The School Management System is a multi-application platform designed to manage academic and administrative operations. It includes four primary user applications:

- Admin Application
- Teacher Application
- Student Application
- Parent Application

Core modules:

- Invoice Management
- Attendance Management
- Notification System
- assessment & Study Programs
- log markes of assessment
- Work Schedules
- teacher & materials
- classes managment
- File Management (PDF, Excel, Documents)

### 1.3 Definitions, Acronyms, Abbreviations

- SRS: Software Requirements Specification
- SMS: School Management System
- API: Application Programming Interface
- JWT: JSON Web Token

### 1.4 References

- Laravel Documentation
- Flutter Documentation
- IEEE 830-1998 Standard

### 1.5 Overview

This document is structured into overall system description, functional and non-functional requirements, external interfaces, and constraints.

---

## 2. Overall Description

### 2.1 Product Perspective

The system follows a Clean Architecture approach and API-First design. The backend exposes RESTful APIs consumed by Flutter mobile applications.

### 2.2 Product Functions

- User Management
- payment system (Manual)
- Attendance Tracking (Manual)
- materials managment
- makres of student
- Notification Delivery (Push Notifications)
- Schedule Management
- assessment Management
- File Upload/Download
- monthly reports

### 2.3 User Classes and Characteristics

| User Class| Description                             |
|-----------|-----------------------------------------|
| Admin     | Full system control                     |
| Teacher   | Manages attendance and academic data    |
| Student   | Views schedules and academic info       |
| Parent    | Monitors student performance & Invoices |

### 2.4 Operating Environment

- Backend: Laravel (PHP)
- Frontend: Flutter (Android & Desctop)
- Database: MySQL
- Server: local_hosting

### 2.5 Design and Implementation Constraints

- Must use Laravel framework
- Must follow Clean Architecture
- Mobile-first design using Flutter

### 2.6 Assumptions and Dependencies

- Stable internet connection
- Availability of smartphones
- Firebase for notifications

---

## 3. External Interface Requirements

### 3.1 User Interfaces

- Mobile UI for all user roles except admin  (Flutter)
- Responsive and user-friendly design

### 3.2 Hardware Interfaces

- Mobile devices (Android / Desctop)

### 3.3 Software Interfaces

- RESTful API (Laravel)
- Firebase Cloud Messaging (Notifications)

### 3.4 Communications Interfaces

- HTTPS protocol
- JSON data format

---

## 4. System Features (Functional Requirements)

### 4.1 User Management

- FR-1: Create user accounts
- FR-2: get user accounts
- FR-3: delete user accounts 
- FR-4: Authenticate users
- FR-5: Assign roles and permissions
- FR-5: display user profile
- FR-5: edite profile

### 4.2 Attendance System

- FR-6: Record attendance manually
- FR-7: send notification to parents
- FR-8: Generate attendance reports

### 4.3 Notification System

- FR-9: Send broadcast notifications
- FR-10: Send targeted notifications
- FR-11: Push notification support

### 4.4 Schedule Management

- FR-10: Create weekly schedules
- FR-10: update weekly schedules
- FR-10: delete weekly schedules
- FR-11: Assign teachers and material in schedules_slots
- FR-12: Display schedules
- FR-11: create period

### 4.5 material Management

- FR-13: Manage material
- FR-14: Assign material to classes
- FR-15: Upload book of material

### 4.6 File Management

- FR-16: Upload files (PDF, Excel, Docs)
- FR-17: Download files

### 4.7 Payment System 

- FR-19: Generate invoices
- FR-20: Record payments
- FR-20: display invoices
- FR-20: get notification when over date to pay 

### 4.7 markes of student 

- FR-20: display markes and final result
- FR-20: make reports

### 4.7 assessment managment

- FR-20: managment assessment
- FR-20: assign markes 

---

## 5. Non-Functional Requirements

### 5.1 Performance

- API response time < 500ms

### 5.2 Security

- Token-based authentication (JWT)
- Role-based access control

### 5.3 Scalability

- Use Redis for caching and queues

### 5.4 Availability

- System uptime ≥ 99%

### 5.5 Maintainability

- Layered codebase following Clean Architecture principles

---

## 6. Other Requirements

### 6.1 Database Requirements

- Relational database design
- Support for transactions

### 6.2 Logging and Monitoring

- Error logging system
- Performance monitoring

---

## 7. Appendices

- ERD diagrams (to be added)
- API documentation (Postman)

---

## ✅ Approval

This document must be reviewed and approved before moving to the design phase.
