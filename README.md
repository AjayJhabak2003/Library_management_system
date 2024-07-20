The Library Management System (LMS) is a software application designed to manage and streamline the operations of a library. It is implemented using C++ and MySQL to handle the database operations. The system is divided into two main modules: Administration and User. This system provides functionalities for adding books, registering students, borrowing books, and displaying available books in the library.

# Key Features:

## Administration Module:

### Add Book: 
Allows the admin to add new books to the library database by providing the book name and quantity.
### Add Student: 
Enables the admin to register new students by entering their student ID.

## User Module:

### Display Available Books:
Displays a list of all the books available in the library.
### Borrow Book: 
Allows registered students to borrow a book from the library. The system checks the availability of the book and updates the quantity accordingly.

# Technical Details:

### Programming Language:
C++
### Database: 
MySQL
### Libraries Used:
<mysql.h> for MySQL database connectivity
<mysqld_error.h> for handling MySQL errors
<windows.h> for system-specific operations like clearing the console screen and sleep functions
<sstream> for string manipulation
Implementation Details:

# Database Connection:

The system connects to a MySQL database using the provided credentials (host, user, password, and database name).
Error handling is implemented to manage connection failures and SQL query errors.
Classes:

## Student Class:
Manages student details (student ID).
## Library Class:
Manages book details (name and quantity).
## Functions:

admin(MYSQL conn, Library l, Student s):* Handles the administration functionalities like adding books and students.
display(MYSQL conn):* Displays the list of available books in the library.
book(MYSQL conn, string Bname):* Checks the availability of a specific book and returns its quantity.
user(MYSQL conn, Library l, Student s):* Manages user operations like borrowing a book after validating the student ID and book availability.

## User Interface:

A console-based user interface is implemented to interact with the admin and users, allowing them to navigate through the system and perform various operations.
Conclusion:

The Library Management System is a robust and efficient application that simplifies library operations. It ensures proper management of books and students, providing a seamless experience for both administrators and users. This project demonstrates proficiency in C++ programming, MySQL database handling, and system integration, making it a valuable addition to any software development portfolio.
