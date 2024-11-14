

# AuthGuard: Secure Login & Registration System 🔐

## Overview
AuthGuard is a Java-based web application providing secure user authentication and registration functionality. Built using Java Servlets, JSP, and MySQL, this project demonstrates core concepts in secure user management, following the MVC architecture. AuthGuard includes login, registration, and session management features, with a focus on privacy and data protection.

## Features
- **User Registration**: New users can register with unique usernames and secure password storage.
- **Login Authentication**: Authenticates users and initiates sessions upon successful login.
- **Session Management**: Maintains user sessions, allowing access to authenticated-only pages.
- **Secure Password Storage**: Passwords are stored securely, and sensitive data handling follows best practices.

## Tech Stack
- **Backend**: Java, JDBC (Java Database Connectivity)
- **Frontend**: JSP (JavaServer Pages)
- **Database**: MySQL with Apache DBCP for connection pooling
- **Design Pattern**: MVC (Model-View-Controller)

## Project Structure
- **Database Setup**: 
  - `users` table for storing user details like `userId`, `username`, `password`, `email`.
  
- **Packages**:
  - `com.authguard.util`: Contains utility classes like `DataSourceUtil` for database connections and `JdbcTemplate` for SQL execution.
  - `com.authguard.dao`: DAO classes (`UserDAO`, `UserDAOImpl`) for database operations such as registration and verification.
  - `com.authguard.service`: Service layer (`UserService`, `UserServiceImpl`) to manage business logic and data interaction.
  - `com.authguard.to`: Transfer Object (TO) classes for user data.
  - `com.authguard.servlets`: Servlets (`LoginServlet`, `RegisterServlet`) for handling user requests.
  
- **JSP Pages**:
  - `login.jsp`: Login form with fields for username and password.
  - `register.jsp`: Registration form with fields for full name, email, username, and password.
  - `home.jsp`: Authenticated home page with options for updating profile or logging out.



## Usage
- **Register a new user** on the `register.jsp` page.
- **Log in** with valid credentials on the `login.jsp` page to access protected resources.
- **Log out** to end the session securely.

## Challenges and Learnings
This project provided hands-on experience with:
- Secure user authentication and session management in Java.
- Implementing an MVC architecture in a Java web application.
- Efficient database handling using JDBC with connection pooling.

## Future Enhancements
- Implement password encryption for added security.
- Add a password recovery feature.
- Extend the profile management functionalities.

