project:
  name: "Employee Appraisal Management System (EAMS)"
  description: >
    A B.Tech Final Year Project developed using PHP and MySQL for managing
    employee performance appraisals in an organization. This system streamlines
    the appraisal process by enabling employees to submit appraisal requests,
    managers to review them, and administrators to manage employee records and reports.

features:
  - Employee Module:
      - User-friendly login and profile management
      - Submit appraisal requests
      - View appraisal status and history
  - Manager Module:
      - Review employee appraisal requests
      - Provide feedback and approve/reject appraisals
      - Track employee performance
  - Admin Module:
      - Manage employees, departments, and designations
      - Generate and export appraisal reports
      - Dashboard with key statistics
  - General:
      - Role-based access (Employee, Manager, Admin)
      - Secure SQL database integration
      - Easy-to-use web interface

tech_stack:
  frontend: ["HTML5", "CSS3", "JavaScript", "Bootstrap"]
  backend: "PHP (Core PHP)"
  database: "MySQL / MariaDB"
  server: "Apache (XAMPP / WAMP / LAMP)"

installation_setup:
  steps:
    - "Clone the repository:"
    - |
      ```bash
      git clone https://github.com/sachinrmishra/Employee-Appraisal-Management-System.git
      cd Employee-Appraisal-Management-System
      ```
    - "Set up the database:"
    - "Import the provided `eams.sql` file into MySQL using phpMyAdmin or CLI."
    - "Update database connection settings in `config.php`:"
    - |
      ```php
      $host = "localhost";
      $user = "root";
      $password = "";
      $database = "eams";
      ```
    - "Run the project:"
    - "Place the project folder in server root directory (`htdocs` for XAMPP)."
    - "Start Apache and MySQL services."
    - "Open http://localhost/EAMS in a browser."

project_structure: |
  EAMS/
  │── assets/         # CSS, JS, and images
  │── config.php      # Database configuration
  │── index.php       # Entry point
  │── admin/          # Admin module
  │── employee/       # Employee module
  │── manager/        # Manager module
  │── database/       # SQL dump files
  │── README.md       # Project documentation

default_credentials:
  admin:
    username: "admin"
    password: "admin123"
  manager:
    username: "manager"
    password: "manager123"
  employee:
    username: "employee"
    password: "employee123"

future_enhancements:
  - Add role-based analytics dashboards
  - Implement email notifications for appraisal updates
  - Migrate to a modern PHP framework (Laravel/CodeIgniter)
  - Deploy on cloud (AWS / Heroku / Azure)

authors:
  - "Sachin Mishra"
  - "Parth Patel"
  - "Madhvesh Patel"
  - "Akash Prajapati"
