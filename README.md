📌 Project Overview

DAOCRUDApplication is a Java-based User Management System that demonstrates CRUD (Create, Read, Update, Delete) operations using JDBC and MySQL. The project follows the DAO (Data Access Object) pattern, ensuring a structured and maintainable approach to database interactions.

🛠 Tech Stack

Java (JDK 11 or later)

JDBC (Java Database Connectivity)

MySQL (Relational Database)

DAO Pattern (For clean code structure)

Maven (For dependency management)

🔹 Features

✔️ Add Users – Insert new users into the database.✔️ View Users – Retrieve and display all users.✔️ Update Users – Modify existing user details.✔️ Delete Users – Remove users from the database.✔️ DAO Pattern – Ensures separation between business logic and database operations.✔️ Prepared Statements – Prevents SQL injection for secure data handling.

📂 Project Structure

DAOCRUDApplication/
│── src/
│   ├── model/
│   │   ├── User.java
│   ├── dao/
│   │   ├── UserDAO.java
│   │   ├── UserDAOImpl.java
│   ├── Main.java
│── pom.xml (for Maven - optional)

📌 How It Works

1️⃣ The user selects an option from the menu (Add, View, Update, Delete).2️⃣ The DAO Layer interacts with MySQL to perform the required action.3️⃣ The system displays results and confirms success or failure.

🛠 Installation & Setup

Step 1: Clone the Repository

git clone https://github.com/yourusername/DAOCRUDApplication.git
cd DAOCRUDApplication

Step 2: Setup MySQL Database

CREATE DATABASE userdb;
USE userdb;
CREATE TABLE users (
id INT PRIMARY KEY AUTO_INCREMENT,
name VARCHAR(255) NOT NULL,
age INT NOT NULL
);

Step 3: Configure Database Connection

Edit UserDAOImpl.java and update your MySQL credentials:

private static final String URL = "jdbc:mysql://localhost:3306/userdb";
private static final String USER = "your_mysql_username";
private static final String PASSWORD = "your_mysql_password";

Step 4: Run the Application

If using Maven, build and run:

mvn clean install
java -jar target/DAOCRUDApplication.jar

Otherwise, run Main.java in your IDE.

🔹 Future Enhancements

🚀 Convert to a Spring Boot REST API.🚀 Add a GUI using JavaFX or Swing.🚀 Implement Logging & Exception Handling.

📜 License

This project is open-source and available for use. Modify as needed!

📧 Contact

For any questions, feel free to reach out via GitHub Issues.

