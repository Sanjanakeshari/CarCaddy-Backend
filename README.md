# 🚗 CarCaddy - Car Rental Automation System

## 📌 Project Overview
**CarCaddy** is a backend-driven **Car Rental Automation System** designed to streamline and automate core rental operations such as employee management, user handling, rental workflows, and account lifecycle processes.  

This project was developed to improve operational efficiency, reduce manual work, and ensure secure and structured management of rental-related activities.

The system focuses on automating internal management processes with features like employee onboarding, validation, password generation, account deactivation, and exception handling.

---

## 🎯 Objective
The main objective of **CarCaddy** is to build a reliable and scalable backend system for car rental business operations by automating employee-related and rental-support workflows.

It helps in:
- Reducing manual administrative work
- Improving employee account management
- Ensuring proper input validation and error handling
- Supporting structured backend operations for rental management

---

## 🛠️ Tech Stack

### Backend
- **Java**
- **Spring Boot**
- **REST APIs**

### Database
- **MySQL**

### Tools & Utilities
- **Postman** (API Testing)
- **Git & GitHub**
- **Maven**
- **VS Code / IntelliJ IDEA**

---

## 📂 Project Modules

### 1. Employee Management Module
This module handles employee-related backend operations such as:
- Employee registration
- Employee data validation
- Role/department mapping
- Temporary and permanent employee handling
- Employee account lifecycle management

### 2. Rental Module Integration
The Employee Management module is connected with the **Rental Module**, ensuring proper department association and backend workflow support.

### 3. Account Management
Includes automated account-related actions such as:
- Default password generation
- Employee account deactivation
- Temporary employee expiry-based deactivation

### 4. Notification Support
Handles automated email notifications for important events such as:
- Account deactivation alerts
- Employee status changes

### 5. Exception Handling & Validation
Includes robust backend validation and API-level exception handling to improve system reliability and response clarity.

---

## ✨ Key Features

- ✅ Employee Registration System  
- ✅ Input Validation for Employee Records  
- ✅ Default Password Auto-Generation  
- ✅ Account Deactivation for Ex-Employees  
- ✅ Auto-Deactivation for Temporary Employees  
- ✅ Email Notification Support  
- ✅ Structured Database Relationships  
- ✅ REST API-Based Backend Workflow  
- ✅ API Exception Handling  
- ✅ Secure and Organized Data Management  

---

## ⚙️ Functional Workflow

### Employee Registration Flow
1. Admin registers a new employee
2. Employee details are validated
3. Employee record is stored in the database
4. A default password is generated automatically
5. Employee account is activated for system use

### Employee Deactivation Flow
1. Employee leaves the organization or contract expires
2. Account status is updated
3. Account is automatically deactivated
4. Notification email is triggered

### Temporary Employee Handling
1. Temporary employee is added with a validity period
2. System tracks employee active duration
3. Once the expiry condition is met, account is deactivated automatically

---

## 🗃️ Database Design (High-Level)
The project uses a **relational database structure** in MySQL with relationships between employee and rental-support entities.

### Example Entities:
- `Employee`
- `Department / Rental Module`
- `User Account`
- `Notification`
- `Role / Access Control`

### Core Database Concepts Used:
- Primary Keys
- Foreign Keys
- Table Relationships
- Data Validation Constraints

---

## 🔍 API Features
The backend exposes REST APIs for core operations such as:

- Add Employee
- Update Employee Details
- View Employee Records
- Deactivate Employee Account
- Auto Handle Temporary Employee Expiry
- Generate Default Credentials
- Validate Employee Input
- Trigger Email Notifications

---

## 🧪 Testing & Validation
The project includes backend testing and validation for:

- Required field validation
- Invalid input handling
- Duplicate employee record checks
- Account deactivation scenarios
- Temporary employee expiry scenarios
- API error handling
- Exception-based response messages

---

## 📊 Business Impact
This system helps improve internal business operations by:

- Reducing manual employee account management
- Preventing invalid or inconsistent records
- Improving backend process automation
- Supporting secure and maintainable rental business workflows

---

## 🚀 Future Enhancements
Planned future improvements include:

- Frontend dashboard integration
- Role-based authentication and authorization
- JWT-based login security
- Rental booking workflow automation
- Payment and invoice integration
- Admin analytics dashboard
- Real-time employee activity tracking

---

## 📁 Suggested Project Structure

```bash
CarCaddy/
│
├── src/
│   ├── main/
│   │   ├── java/
│   │   │   └── com/carcaddy/
│   │   │       ├── controller/
│   │   │       ├── service/
│   │   │       ├── repository/
│   │   │       ├── entity/
│   │   │       ├── dto/
│   │   │       ├── exception/
│   │   │       └── config/
│   │   └── resources/
│   │       ├── application.properties
│   │       └── templates/
│
├── pom.xml
├── README.md
└── .gitignore
