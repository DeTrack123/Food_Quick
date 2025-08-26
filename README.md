# Poised Project Management System

The **Poised Project Management System** is a Java-based console application designed to manage construction projects.  
It allows users to **add**, **update**, **delete**, **finalise**, and **search projects**, while also providing reports on **incomplete** and **overdue projects**.

---

## Features

- **Add New Project** → Capture project details and save them in the database.
- **Update Project** → Edit project details such as deadlines or customer info.
- **Delete Project** → Remove projects permanently.
- **Finalise Project** → Mark projects as completed and generate invoices if needed.
- **View Incomplete Projects** → List all ongoing projects.
- **View Overdue Projects** → Identify projects past their deadlines.
- **Find Project by Number/Name** → Search projects using project number or project name.

---

## Technologies Used

- **Java (JDK 11+)**
- **JDBC** for database operations
- **MySQL** as the database
- **Javadoc** for API documentation

---

## Project Structure

poised-project/
├── poisedMain.java # Entry point with menu and user input handling.
├── ProjectManager.java # Handles all project database operations.
├── README.md # Project documentation.
└── /doc # Generated Javadoc output.

---

## Getting Started

### Database setup

- Ensure MySQL is installed and running.
- Create a database.
- Import your project table schema.
- Update ProjectManager.java with your database credentials:
- Connection conn = DriverManager.getConnection( - "jdbc:mysql://localhost:3306/poisedpms?useSSL=false", - "your-username",
  = "your-password"
  );

---

### Example Menu

When running, you’ll see:

--- Poised Project Management ---

1. Add New Project
2. Update Project
3. Delete Project
4. Finalise Project
5. View Incomplete Projects
6. View Overdue Projects
7. Find Project by Number/Name
8. Exit
   Enter choice:

---

### Best Practices Followed

- Proper exception handling with try-catch.
- Code comments explaining each method.
- Scanner closed safely using try-with-resources.
- Separation of concerns: poisedMain (UI & menu) vs ProjectManager (DB logic).
- Javadoc-ready methods with @param, @return, and @throws.

---

### Author

- Christo Swanepoel
- Principal Measurement Technician & Software Development Student
- [christo.swanepoeljc@gmail.com]
