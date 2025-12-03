
# 🌐✨🚀 **𝙅𝙤𝙗𝙋𝙤𝙧𝙩𝙚𝙡** 🚀✨🌐  
### _Full-Stack Job Portal Application_  
**Created By: SHAIK SADIK**

<img src="https://img.shields.io/badge/Frontend-React%20%2B%20Vite-blue?style=for-the-badge">
<img src="https://img.shields.io/badge/Backend-SpringBoot-green?style=for-the-badge">
<img src="https://img.shields.io/badge/Database-MySQL-orange?style=for-the-badge">

---


</div>

---

## 🌐 Live Demo
🔗 **Frontend (Vercel Deployment):** Not hosted (local setup only)

🛑 **Backend & MySQL:** Not hosted (local setup only)

---

## 📌 About the Project
JobPortel is a modern full-stack job portal system showcasing UI → API → Database communication.  
Includes:

- React + Vite frontend  
- Spring Boot backend  
- MySQL database  

---

## 🚀 Tech Stack

### Frontend  
- React  
- Vite  
- Axios  
- JavaScript / JSX  

### Backend  
- Spring Boot  
- Spring Web  
- JPA / Hibernate  
- MySQL Connector  

### Database  
- MySQL 8+

---

## 📂 Project Structure

```

JobPortel/
│
├── jobportal frontend/
│   └── jobportal/
│       ├── public/
│       ├── src/
│       ├── package.json
│       ├── vite.config.js
│       └── index.html
│
└── JobPortal/
└── JobPortal/
├── src/main/java/
├── src/main/resources/
│    └── application.properties
├── pom.xml
└── README-backend.md

```

---

## 🖼 Screenshot Grid

Place images here:

```

jobportal frontend/jobportal/public/

````

<div align="center">

<table>
<tr>
<td><img src="./jobportal%20frontend/jobportal/public/screenshot1.png" width="350"></td>
<td><img src="./jobportal%20frontend/jobportal/public/screenshot2.png" width="350"></td>
</tr>
</table>

</div>

---

# 🛠 Running the Project Locally

## ✔️ Clone Repo

```bash
git clone https://github.com/sadikshaik01/JobPortel.git
cd JobPortel
````

---

## ✔️ MySQL Setup

```sql
CREATE DATABASE jobportel_db;

CREATE USER 'jobuser'@'localhost' IDENTIFIED BY 'jobpass';

GRANT ALL PRIVILEGES ON jobportel_db.* TO 'jobuser'@'localhost';
FLUSH PRIVILEGES;
```

---

# 🔧 Backend Setup (Spring Boot)

## ✔️ Navigate to Backend

```bash
cd JobPortal/JobPortal
```

## ✔️ Configure application.properties

```properties
spring.datasource.url=jdbc:mysql://localhost:3306/jobportel_db
spring.datasource.username=jobuser
spring.datasource.password=jobpass

spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=true
spring.jpa.database-platform=org.hibernate.dialect.MySQL8Dialect

server.port=8080
```

## ✔️ Run Backend

```bash
./mvnw spring-boot:run
```

OR

```bash
mvn spring-boot:run
```

Backend Runs At:
**[http://localhost:8080](http://localhost:8080)**

---

# 💻 Frontend Setup (React + Vite)

## ✔️ Navigate to Frontend

```bash
cd "jobportal frontend/jobportal"
```

## ✔️ Install Dependencies

```bash
npm install
```

## ✔️ Add .env File

```
VITE_API_BASE_URL=http://localhost:8080
```

## ✔️ Start Dev Server

```bash
npm run dev
```

Frontend Runs At:
**[http://localhost:5173](http://localhost:5173)**

---

# 📘 API Documentation

> Modify based on your backend controllers.

### ✔️ Get All Jobs

```
GET /jobs
```

### ✔️ Create Job

```
POST /jobs
{
  "title": "Software Engineer",
  "company": "ABC",
  "location": "Hyderabad"
}
```

### ✔️ Delete Job

```
DELETE /jobs/{id}
```

---

# 🗄 Database ER Diagram

```
+-------------+         +----------------+
|   USERS     | 1 --- n |     JOBS       |
+-------------+         +----------------+
| id (PK)     |         | id (PK)        |
| username    |         | title          |
| email       |         | company        |
| password    |         | location       |
+-------------+         +----------------+
```


---

<div align="center">

# 🏆 **Credits**

### 💡 Project: **JobPortel**

### 👨‍💻 Developer: **SHAIK SADIK**

Built with ❤️ dedication, passion & learning.

⭐ If you like this project, don’t forget to star the repo! ⭐

</div>

```


