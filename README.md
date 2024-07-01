# Patient Record Management System

## Overview
The Patient Record Management System is a Java-based application built to manage patient records efficiently. It allows users to perform CRUD (Create, Read, Update, Delete) operations on patient information stored in a MySQL database managed through XAMPP. The system provides functionalities for searching patients by phone number, displaying their details, and deleting records as needed.

## Features
- **Search by Phone Number:** Enables users to search for patient records using their phone number.
- **Display Patient Details:** Retrieves and displays patient information including name, age, and address.
- **Delete Patient Records:** Provides an option to delete patient records from the database based on the phone number.
- **Validation Checks:** Implements validation to ensure correct input formats and prevent errors during data retrieval and deletion operations.

## Technologies Used
- **Java:** Used for the application logic and GUI development using NetBeans IDE.
- **MySQL:** Database management system used to store and retrieve patient records via XAMPP.
- **Swing:** Java GUI widget toolkit used for creating the graphical user interface.
- **JDBC:** Java Database Connectivity for connecting Java applications with MySQL databases.

## Prerequisites
1. **XAMPP:** Install XAMPP, which includes MySQL, Apache, and PHP.
   - Download XAMPP from [https://www.apachefriends.org/index.html](https://www.apachefriends.org/index.html)
   - Start the Apache and MySQL services using the XAMPP control panel.

## Installation
1. **Clone Repository:**
   ```bash
   git clone <repository_url>
   ```
   
2. **Import Project into NetBeans:**
   - Open NetBeans IDE.
   - Select **File -> Open Project** and navigate to the cloned repository directory.
   - Select the project folder and click **Open Project**.

3. **Set Up MySQL Database with XAMPP:**
   - Start XAMPP and ensure Apache and MySQL services are running.
   - Open a web browser and go to `http://localhost/phpmyadmin`.
   - Create a database named `employee_db`.
   - Create a table named `employee` with columns:
     - `Phone` (VARCHAR or INT, depending on your preference)
     - `Password` (VARCHAR)
     - `Name` (VARCHAR)
     - `Address` (VARCHAR)
     - `Age` (INT)

4. **Configure Database Connection:**
   - Modify the database connection details in `DB_Connection.java` to match your XAMPP MySQL server configuration (`DB_URL`, `USER`, `PASS`). Example:
   ```java
   static final String DB_URL = "jdbc:mysql://localhost/employee_db";
   static final String USER = "root";
   static final String PASS = "";
   ```

5. **Build and Run:**
   - Build the project in NetBeans.
   - Run the application to start the Patient Record Management System.

## Usage
- **Search for Patients:**
  Enter a valid phone number in the search field and click the **Search** button to retrieve patient details.

- **Delete Patient Records:**
  After searching for a patient, click the **Delete** button to delete their record from the database after confirmation.

## Contributing
Contributions are welcome. If you find any issues or have suggestions for improvements, please open an issue or submit a pull request.

