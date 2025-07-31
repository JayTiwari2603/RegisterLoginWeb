# 🚀 Register & Login Web Application (Java, Servlet, JSP, JDBC, MySQL)

This is a full-stack Java web application built using **Servlets**, **JSP**, **JDBC**, and **MySQL** to handle user **registration** and **login** functionality. It demonstrates a clean MVC structure, DAO pattern, session handling, and dynamic response rendering.

---

## 🌐 Features

- ✅ User Registration
- ✅ User Login with Session
- ✅ Logout functionality
- ✅ Authentication check with session management
- ✅ JDBC-based database operations
- ✅ Clean & responsive UI using HTML & CSS
- ✅ DAO Layer abstraction

---

## 🛠️ Technologies Used

| Layer        | Technology                |
|--------------|----------------------------|
| Frontend     | HTML, CSS, JSP             |
| Backend      | Java Servlets              |
| Database     | MySQL                      |
| Connectivity | JDBC                       |
| Build Tool   | Manual / IDE based         |
| Server       | Apache Tomcat (Recommended v10+) |

---


---

## 🧠 How It Works

1. **Home Page (`index.html`)** – Welcome page with links to Login or Register.
2. **Register** – Collects `username`, `email`, `password`, and stores in the MySQL DB.
3. **Login** – Authenticates against stored user credentials.
4. **Welcome Page** – Protected page only visible if logged in (via session).
5. **Logout** – Destroys session and redirects to homepage.

---

## 🧪 Database Setup

1. Create a MySQL database:
```sql
CREATE DATABASE registerlogin;

2. Create users table:
CREATE TABLE users (
  id INT AUTO_INCREMENT PRIMARY KEY,
  username VARCHAR(100) NOT NULL,
  email VARCHAR(100),
  password VARCHAR(100) NOT NULL
);

3.Update your DB credentials in DBUtil.java:
private static final String URL = "jdbc:mysql://localhost:3306/registerlogin";
private static final String USERNAME = "your_username";
private static final String PASSWORD = "your_password";

▶️ How to Run
Import project into Eclipse or IntelliJ IDEA.

Add MySQL JDBC Driver (mysql-connector-j.jar) to WEB-INF/lib.

Configure Apache Tomcat in your IDE.

Deploy the project and run on http://localhost:8080/RegisterLoginApp.

🙌 Author
Jayantkumar Tiwari
Aspiring Full-Stack Java Developer




