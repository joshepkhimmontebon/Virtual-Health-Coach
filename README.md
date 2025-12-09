# Virtual-Health-Coach
Virtual Health Coach - A comprehensive healthcare management web application featuring symptom tracking, FAQ database, doctor consultations, and user authentication. Built with PHP, MySQL, and responsive design. Complete CRUD operations with role-based access for patients and healthcare providers.


<img width="1333" height="629" alt="Website Picture" src="https://github.com/user-attachments/assets/85508e84-c1dc-47ef-9781-1ff627d4ec7d" />


Virtual Health Coach - Healthcare Management System

📋 Overview

Virtual Health Coach is a comprehensive web-based healthcare management platform designed to facilitate communication between patients and healthcare providers. The application enables users to track symptoms, access healthcare education, view FAQs, and receive professional medical advice from doctors.

✨ Key Features

👥 User Management
- Dual Role System: Separate interfaces for patients and healthcare professionals
- Secure Authentication: Password hashing with bcrypt and session-based authentication
- User Profile: Complete user information management with editable details
- Role-Based Access Control: Different features and permissions for patients vs. doctors

🔍 Symptom Tracking Module
- Log and track health symptoms with detailed information
- Record symptom date, duration, and lifestyle factors
- View personal symptom history
- Edit and delete symptom records
- Search and filter functionality

📚 FAQ Management System
- Comprehensive FAQ database for healthcare education
- Doctors can add, edit, and delete FAQ entries
- Patients can search and view relevant FAQs
- Accordion-style interface for easy navigation
- Pre-populated with healthcare topics (cough, fever, common cold, etc.)

👨‍⚕️ Doctor Dashboard
- View all registered patients
- Access detailed patient information
- Monitor patient symptoms
- Provide medical advice and recommendations
- Manage FAQ content

📖 Healthcare Education
- Educational resources for users
- Doctor-provided healthcare content
- Quick access to medical information

💬 Contact & Support
- Contact form for user inquiries
- Support section for common issues

🗄️ Database Architecture

MySQL Schema (user_db)

4 Main Tables:

1. user_form - User/Doctor accounts with credentials and profiles
2. tbl_faq - Frequently Asked Questions and answers
3. symptoms - User symptom tracking and history
4. doctors_advice - Doctor recommendations and medical advice

Databade Table Diagrams

<img width="1024" height="1536" alt="ERD FINAL" src="https://github.com/user-attachments/assets/c138291b-6c9e-43d8-a727-eaac4b44e9e8" />


🔧 Technology Stack

- Backend: PHP (MySQLi & PDO)
- Database: MySQL
- Frontend: HTML5, CSS3, JavaScript
- Architecture: MVC-style with separated concerns
- Security: Prepared statements, password hashing, session management

📊 CRUD Operations

✅ Create
- User registration with validation
- Add new FAQs (doctor only)
- Log new symptoms
- Create doctor's advice records

✅ Read
- View all FAQs with search
- Display symptom history
- View user profiles
- Doctor patient list and details

✅ Update
- Edit FAQ entries
- Update symptom records
- Modify user profile information
- Update doctor information

✅ Delete
- Remove FAQ entries
- Delete symptom records
- User account removal

🚀 Getting Started

Prerequisites
- XAMPP (or similar PHP/MySQL environment)
- PHP 7.4+
- MySQL 5.7+
- Web browser (Chrome, Firefox, Safari, Edge)

Installation

1. Create Database
   ```sql
   CREATE DATABASE user_db;
   ```

2. Import SQL Files
   - Import `database/user_form.sql`
   - Import `database/tbl_faq.sql`
   - Import `database/symptoms.sql`
   - Import `database/doctors_advice.sql`

3. Configure Database Connection
   - Update credentials in `config.php` and `conn.php`
   - Default: localhost, user: root, password: 123ABC12

4. Access Application
   - Navigate to: `http://localhost/user-type/home.php`

🔒 Security Features

- Password Security: bcrypt hashing (PASSWORD_DEFAULT)
- SQL Injection Prevention: Prepared statements with parameterized queries
- Session Management: Secure session-based authentication
- Input Validation: Form validation and sanitization
- Access Control: Role-based permissions for users and doctors
- Error Handling: Comprehensive exception handling with user-friendly messages

📁 Project Structure

Healthcare/user-type/
├── database/                  # SQL schema files
├── config.php                 # MySQLi connection
├── conn.php                   # PDO connection
├── home.php                   # Landing page
├── login_form.php             # Authentication
├── register.php               # User registration
├── user_page.php              # User dashboard
├── sc.php                     # Symptom checker
├── faq.php                    # FAQ viewer
├── add-faq.php                # Create FAQ (admin)
├── update-faq.php             # Edit FAQ (admin)
├── delete-faq.php             # Delete FAQ (admin)
├── doctor_page.php            # Doctor dashboard
├── sc_doc.php                 # Doctor's symptom view
├── view_details.php           # Patient details (doctor view)
├── he.php                     # Healthcare education
├── ca.php                     # Contact us
├── css/                       # Stylesheets
└── js/                        # JavaScript files

📝 Features by Module

| Module | Features | Users |
|--------|----------|-------|
| **Authentication** | Login, Register, Session Management | All |
| **Symptom Checker** | Log, View, Edit, Delete, Search | Patients |
| **FAQ Management** | View, Search | All; Create/Edit/Delete: Doctors |
| **User Profile** | View, Edit Details | All |
| **Doctor Dashboard** | View Patients, Add Advice | Doctors |
| **Healthcare Education** | Educational Content | All |
| **Contact** | Send Messages | All |

🎯 Learning Outcomes

This project demonstrates:
- ✅ Relational database design and normalization
- ✅ Full CRUD operation implementation
- ✅ Secure backend development with PHP
- ✅ Session-based authentication
- ✅ Security best practices
- ✅ Responsive web design
- ✅ Role-based access control
- ✅ Error handling and validation

📋 Academic Compliance

This application fulfills all requirements for database integration coursework:
- ✅ MySQL relational database schema
- ✅ Complete CRUD operations
- ✅ PHP backend routes
- ✅ Functional frontend UI
- ✅ Comprehensive documentation
- ✅ Security implementation
- ✅ Test data and credentials
