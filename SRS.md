# Software Requirements Specification (SRS)
## Hotel Management System
SWE202 – Software Modeling and Design

---

# 1. Introduction

## 1.1 Purpose

This document defines the functional and non-functional requirements of the Hotel Management System. It serves as the foundation for system modeling and design.

## 1.2 Scope

The system automates hotel operations including:

- Room management
- Reservation handling
- Guest check-in and check-out
- Payment processing
- Reporting and statistics

---

# 2. Overall Description

## 2.1 Product Perspective

The system is a standalone application that centralizes hotel operations into a digital platform, replacing manual booking and billing processes.

## 2.2 User Classes

### Guest
- Search rooms
- Make and manage reservations
- Make payments

### Receptionist
- Manage check-in/check-out
- Assign rooms
- Generate invoices

### Manager
- Manage rooms and pricing
- View reports and statistics

### Administrator
- Manage system users
- Configure system settings

---

# 3. Functional Requirements

## 3.1 Authentication & User Management

FR-01: The system shall allow users to log in using username and password.  
FR-02: The system shall support role-based access control.  
FR-03: The system shall allow administrators to create user accounts.  
FR-04: The system shall allow administrators to update user accounts.  
FR-05: The system shall allow administrators to deactivate user accounts.  
FR-06: The system shall log user activities.

## 3.2 Room Management

FR-07: The system shall allow managers to add rooms.  
FR-08: The system shall allow managers to edit room details.  
FR-09: The system shall allow managers to delete rooms.  
FR-10: The system shall store room status (Available, Occupied, Reserved, Cleaning, Maintenance).  
FR-11: The system shall automatically update room status after check-in and check-out.  
FR-12: The system shall prevent double booking of rooms.

## 3.3 Reservation Management

FR-13: The system shall allow guests to search available rooms by date.  
FR-14: The system shall allow filtering by room type and price range.  
FR-15: The system shall allow guests to create reservations.  
FR-16: The system shall allow guests to cancel reservations.  
FR-17: The system shall allow modification of reservations.  
FR-18: The system shall calculate total cost automatically.  
FR-19: The system shall generate reservation confirmations.  
FR-20: The system shall send booking confirmation via email.

## 3.4 Check-in / Check-out

FR-21: The system shall allow receptionists to check in guests.  
FR-22: The system shall assign rooms during check-in.  
FR-23: The system shall record guest identification details.  
FR-24: The system shall allow receptionists to check out guests.  
FR-25: The system shall generate invoices at check-out.  
FR-26: The system shall update room status to "Cleaning" after check-out.

## 3.5 Payment Management

FR-27: The system shall support multiple payment methods (cash, card, online).  
FR-28: The system shall record payment transactions.  
FR-29: The system shall generate payment receipts.  
FR-30: The system shall allow partial payments.  
FR-31: The system shall store payment history.

## 3.6 Reporting & Management

FR-32: The system shall generate daily revenue reports.  
FR-33: The system shall generate monthly occupancy reports.  
FR-34: The system shall allow managers to view booking statistics.  
FR-35: The system shall allow export of reports in PDF format.  
FR-36: The system shall display real-time room availability dashboard.

---

# 4. Non-Functional Requirements

NFR-01: The system shall respond within 2 seconds.  
NFR-02: The system shall ensure data integrity and consistency.  
NFR-03: The system shall encrypt user passwords.  
NFR-04: The system shall support at least 100 concurrent users.  
NFR-05: The system shall ensure secure data storage and controlled access.
