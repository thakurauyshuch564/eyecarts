# 📘 Product Requirements Document (PRD)

## Clinic Management System

**Tech Stack:** React.js (Frontend) + Supabase (Backend & Database)

---

## 1. Project Overview

The Clinic Management System is a web-based application designed to automate and manage daily clinic operations such as patient registration, doctor management, appointment scheduling, billing, and reports. The system supports role-based access for Admin, Doctor, and Patient.

---

## 2. Objectives

* Digitize clinic workflows
* Reduce manual paperwork
* Provide secure role-based access
* Enable real-time appointment management
* Centralize patient medical records

---

## 3. User Roles

### 3.1 Admin

* Manage doctors and staff
* View all appointments
* Manage billing & reports
* System configuration

### 3.2 Doctor

* View assigned appointments
* Access patient records
* Add diagnosis & prescriptions

### 3.3 Patient

* Register & login
* Book appointments
* View prescriptions & bills

---

## 4. System Modules

1. Authentication Module
2. Patient Management
3. Doctor Management
4. Appointment Scheduling
5. Billing & Payments
6. Reports & Dashboard

---

## 5. Functional Requirements

### Authentication

* Email/password login (Supabase Auth)
* Role-based redirection

### Patient Management

* Add / update patient profile
* View medical history

### Doctor Management

* Add doctor details
* Assign specialization & availability

### Appointment Management

* Book appointment
* Approve / reject appointment
* Status tracking

### Billing

* Generate bill
* Payment status (Paid / Pending)

---

## 6. Non-Functional Requirements

* Secure authentication
* Responsive UI
* Scalable database design
* Fast performance

---

## 7. Database Design (Supabase)

### Tables

**users**

* id (uuid)
* role (admin / doctor / patient)

**patients**

* patient_id (uuid)
* name
* age
* gender
* contact
* user_id (FK)

**doctors**

* doctor_id (uuid)
* name
* specialization
* availability
* user_id (FK)

**appointments**

* appointment_id (uuid)
* patient_id (FK)
* doctor_id (FK)
* date
* time
* status

**billing**

* bill_id (uuid)
* appointment_id (FK)
* amount
* payment_status

---

## 8. Frontend (React.js)

### Pages

* Login / Register
* Admin Dashboard
* Doctor Dashboard
* Patient Dashboard
* Appointment Booking
* Billing Page

### Libraries

* React Router
* Axios
* Supabase JS SDK

---

## 9. Backend (Supabase)

* Supabase Auth for login
* PostgreSQL database
* Row Level Security (RLS)
* Supabase APIs for CRUD

---

## 10. Application Flow

1. User registers / logs in
2. Role-based dashboard loads
3. Patient books appointment
4. Doctor updates consultation
5. Bill generated
6. Admin monitors reports

---

## 11. Prompt (For AI / Documentation / Viva)

> "Design and develop a Clinic Management System using React.js for frontend and Supabase for backend and database. The system should support Admin, Doctor, and Patient roles, enable appointment booking, patient record management, billing, and secure authentication with role-based access control."

---

## 12. Future Enhancements

* SMS / Email notifications
* Online payment gateway
* Prescription download (PDF)
* Analytics dashboard

---

## 13. Conclusion

The Clinic Management System provides a complete digital solution for managing clinic operations efficiently and securely using modern web technologies.

---

✅ Suitable for **college projects, internships, viva, and real-world demo**
