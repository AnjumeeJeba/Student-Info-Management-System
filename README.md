# Student-Info-Management-System
A Java Swing application to manage student records using a GUI. This project demonstrates how to perform basic CRUD (Create, Read, Update, Delete) operations with a student database table, showcasing integration with a relational database using JDBC.

## Features
- Add New Records: Insert student details (Name, Roll Number, Age) into the database.
- View Records: Navigate through the student database using First, Next, Previous, and Last buttons.
- Update Records: Modify the existing student information in the database.
- Delete Records: Remove student details from the database.
- Reset Form: Clear all text fields to enter new details.
- Database Integration: Uses JDBC for database connectivity.

## Technologies Used
*Java Swing*: For GUI components.
*JDBC*: For database communication.
*Java SE*: Core Java libraries.

Prerequisites
- Java Development Kit (JDK) 8 or later.
- A relational database like MySQL or PostgreSQL installed.
- A database table named student with the following schema:
```sql
CREATE TABLE student (
    id INT PRIMARY KEY AUTO_INCREMENT,
    Name VARCHAR(100),
    Rollnum VARCHAR(50),
    Age INT
);
```

## Installation & Setup
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/studentinfo.git
   cd studentinfo

3. Import the project into your favorite Java IDE (e.g., IntelliJ IDEA, Eclipse, NetBeans).
4. Configure the database connection:
      - Modify the connectToDatabase method to include your database credentials:
   ```java
   private Connection connectToDatabase() throws SQLException {
    return DriverManager.getConnection("jdbc:mysql://localhost:3306/your_database", "your_username", "your_password");}
   
6. Build and run the project:
    - Compile the code and execute the main method in the studentinfo class.

# Usage
1. Launch the application by running the main method in studentinfo.java.
2. Use the following buttons to interact with the application:
    - First: View the first record.
    - Next: View the next record.
    - Previous: View the previous record.
    - Last: View the last record.
    - Insert: Add a new record to the database.
    - Update: Modify the selected record.
    - Delete: Remove the selected record.
    - Reset: Clear the form fields.
