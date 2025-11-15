# CETM74-Assignment2-ITRequestSystem
Web-based IT Request Management System for WearView Academy using PHP, MySQL, HTML, CSS, and JavaScript.

**Module:** CETM74 – Web Design & Development  
**Author:** Maryam Akhtar  
**Degree:** MSc Computer Science (Graduating 2026)  
**Institution:** WearView Academy (Prototype Scenario)  

---

## Project Overview
This project extends the prototype created in **Assignment 1** into a **fully functional IT Request Management System** for WearView Academy.  
The system allows staff to report IT issues and enables technicians to view, manage, and complete these requests.

The aim was to develop a working web application with:
- Server-side functionality using **PHP**
- A connected **MySQL database**
- **Client-side and server-side validation**
- Role-based login redirection for staff and technicians
- A responsive and accessible design suitable for multiple devices

---

## Key Features

### Staff Users
- Login with a shared staff username and password  
- Access a form to report IT issues  
- Validation ensures all required fields are complete and email format is correct  
- Submitted data is stored securely in a MySQL database  

### Technician Users
- Login using a technician password  
- Redirected to a portal displaying incomplete and completed jobs  
- Ability to update a job’s status (mark as complete/incomplete)  
- All job records dynamically loaded from the database  

---

## Technology Stack

| Layer | Technology |
|--------|-------------|
| Front-End | HTML5, CSS3, JavaScript |
| Server-Side | PHP |
| Database | MySQL |
| Tools | XAMPP, phpMyAdmin, Visual Studio Code |
| Validation | Client-side (JavaScript) & Server-side (PHP) |

---

## Database Structure

**Database Name:** `it_support`  
**Table Name:** `t_itrequest`

| Column | Type | Description |
|---------|------|-------------|
| `request_id` | INT (Primary Key, AUTO_INCREMENT) | Unique ID for each request |
| `staff_name` | VARCHAR(100) | Name of staff reporting the issue |
| `email` | VARCHAR(100) | Staff email address |
| `room_number` | VARCHAR(20) | Location of issue |
| `issue_description` | TEXT | Description of IT fault |
| `status` | VARCHAR(20) | “Incomplete” or “Complete” |
| `date_reported` | DATETIME | Timestamp of submission |

---

## Functionality Summary

-  **Login system** for staff and technician roles  
-  **Report form** to log IT issues  
-  **Database integration** with insert, update, and fetch operations  
-  **Technician dashboard** for status updates  
- **Responsive design** suitable for desktop, tablet, and mobile  

---

##  Testing (Part B)

A total of **15 tests** were carried out to ensure functionality, covering:

| Test No. | Description | Expected Result | Outcome |
|-----------|--------------|----------------|----------|
| 1 | Staff login (valid credentials) | Redirects to staff form | ✅ Pass |
| 2 | Technician login (valid credentials) | Redirects to job list | ✅ Pass |
| 3 | Invalid login | Displays error message | ✅ Pass |
| 4 | Blank form submission | Shows validation error | ✅ Pass |
| 5 | Invalid email format | Prevents submission | ✅ Pass |
| 6 | Database insert | Record stored successfully | ✅ Pass |
| 7 | Update job status | Changes saved to database | ✅ Pass |

*(Full table available in `Part B and Part C - Maryam Akhtar.pdf`)*

---

##  Critical Evaluation (Part C)

The critical evaluation reflects on:
- **Strengths:** Functionality, accessibility, usability, and code structure  
- **Weaknesses:** Basic authentication, manual testing  
- **Future Improvements:**
  - Session-based authentication  
  - Encrypted login credentials  
  - Email notifications for new IT requests  
  - Filter options for job lists  

*(See full evaluation in `Part B and Part C - Maryam Akhtar.pdf`)*

---

