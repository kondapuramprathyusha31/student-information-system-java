# 🎓 Student Information Management System

A desktop-based Student Information Management System developed using **Java Swing, JDBC, and MySQL**. The application provides a graphical interface to manage student records efficiently, with features for adding, viewing, updating, deleting, and searching student information.

## 📌 Project Overview

The Student Information Management System simplifies the process of maintaining student records in a database. It combines Java's object-oriented programming capabilities, Swing GUI components, JDBC database connectivity, and MySQL data storage in one application.

## ✨ Features

- **Add Students:** Register new students with their details.
- **View Students:** Display student records in a table.
- **Update Records:** Modify existing student information.
- **Delete Records:** Remove selected student records.
- **Search Students:** Find records using the available search functionality.
- **Table Sorting:** Sort student records using table columns.
- **Statistics Dashboard:** View student statistics.
- **Input Validation:** Validate entered data before processing.
- **Graphical User Interface:** Interact with the system through a Java Swing desktop application.
- **Database Connectivity:** Store and retrieve records using MySQL and JDBC.

## 🛠️ Technologies Used

| Technology | Purpose |
|---|---|
| Java | Application logic and object-oriented programming |
| Java Swing | Desktop graphical user interface |
| JDBC | Connecting Java to the database |
| MySQL | Storing student records |
| MySQL Connector/J | JDBC driver for MySQL |
| Visual Studio Code | Development environment |
| Git and GitHub | Version control and project hosting |

## 📂 Project Structure

```text
Student-Information-Management-System/
├── src/
│   ├── DBConnection.java
│   ├── StudentDAO.java
│   └── StudentManagementGUI.java
├── lib/
│   └── mysql-connector-j-*.jar
├── out/                 # Generated compiled files
├── .gitignore
└── README.md
```

## ⚙️ Prerequisites

Before running the project, install or configure:

- Java Development Kit (JDK)
- MySQL Server
- MySQL Connector/J
- Visual Studio Code or another Java-compatible IDE

## 🗄️ Database Setup

### 1. Create the database

Open MySQL Workbench or the MySQL command-line client and execute:

```sql
CREATE DATABASE student_db;

USE student_db;

CREATE TABLE students (
    student_id INT PRIMARY KEY AUTO_INCREMENT,
    name VARCHAR(100) NOT NULL,
    age INT,
    gender VARCHAR(20),
    department VARCHAR(100),
    email VARCHAR(100),
    phone VARCHAR(15)
);
```

### 2. Configure database connectivity

Open `src/DBConnection.java` and verify that the connection settings match your local MySQL configuration.

Database URL:

```text
jdbc:mysql://localhost:3306/student_db
```

Use your own local MySQL username and password. **Never publish your database password or other credentials on GitHub.**

### 3. Verify the JDBC driver

Ensure the MySQL Connector/J JAR file is available inside the `lib` directory.

## ▶️ How to Run the Project

### Step 1: Open the project

Open the `Student-Information-Management-System` folder in Visual Studio Code.

### Step 2: Open the terminal

Open **Terminal → New Terminal** in VS Code.

### Step 3: Compile the Java source files

Run the following command from the project root directory:

```powershell
javac -cp "lib\*" -d out src\DBConnection.java src\StudentDAO.java src\StudentManagementGUI.java
```

### Step 4: Launch the application

```powershell
java -cp "out;lib\*" StudentManagementGUI
```

The Student Information Management System window should open. Ensure that MySQL Server is running before using database operations.

## 🧪 Testing

The following application functions have been tested:

- [x] Add student
- [x] View all students
- [x] Update student
- [x] Delete student
- [x] Search student
- [x] Sort table records
- [x] View statistics
- [x] Validate input

## 🎯 Project Objectives

- Apply object-oriented programming concepts in Java.
- Develop a desktop application using Java Swing.
- Establish database connectivity using JDBC.
- Perform CRUD operations on a MySQL database.
- Improve data management through search, sorting, and validation.
- Build practical software development and database management skills.

## 🔮 Future Enhancements

- User authentication and role-based access.
- Student attendance management.
- Report generation and export.
- Student performance and marks management.
- Backup and restore functionality.

## 👩‍💻 Author

**KONDAPURAM PRATHYUSHA**

GitHub: [kondapuram prathyusha31](https://github.com/kondapuramprathyusha31)

## 📄 License

No license has been specified for this project yet. A license can be added if you decide to distribute the project for reuse.

---

⭐ If you find this project useful, consider starring the repository.

