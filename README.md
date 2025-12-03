# JobPortel

> A full-stack Job Portal application  
> **Created By: SHAIK SADIK**  
> Frontend built using **React (Vite)**, Backend using **Spring Boot**, Database using **MySQL**  

![Tech Stack](https://img.shields.io/badge/Frontend-React%20%2B%20Vite-blue?style=for-the-badge)
![Backend](https://img.shields.io/badge/Backend-SpringBoot-green?style=for-the-badge)
![Database](https://img.shields.io/badge/Database-MySQL-orange?style=for-the-badge)

---

## 🌐 Live Demo
**Frontend (Vercel Deployment):**  
🔗 https://___________ *(replace with your actual link)*

**Backend & MySQL:**  
🛑 Not hosted — available for local setup only.

---

## 📌 About the Project
JobPortel is a simple job-listing platform designed to demonstrate a working full-stack flow — from UI → API → Database.  
The project is divided into:

- **React + Vite frontend** (Vercel-ready)
- **Spring Boot backend**
- **MySQL database**

---

## 🚀 Tech Stack

### **Frontend**
- React  
- Vite  
- Axios  
- JavaScript / JSX  

### **Backend**
- Spring Boot  
- Spring Web  
- MySQL Connector  
- JPA / Hibernate  

### **Database**
- MySQL 8+

---

## 📁 Project Structure (Based on Your Repo)


JobPortel/
│
├── jobportal frontend/
│ └── jobportal/ # React + Vite frontend
│ ├── public/ # Add 2 screenshots here
│ ├── src/
│ ├── package.json
│ ├── vite.config.js
│ └── index.html
│
└── JobPortal/
└── JobPortal/ # Spring Boot backend
├── src/main/java/
├── src/main/resources/
│ └── application.properties
├── pom.xml
└── README-backend.md


---

## 🖼 Screenshots

(Add two pictures to the frontend `public` folder and rename them as below)



Then they will appear here ↓

![Screenshot 1](./jobportal%20frontend/jobportal/public/screenshot1.png)
![Screenshot 2](./jobportal%20frontend/jobportal/public/screenshot2.png)

---

# 🛠️ Running the Project Locally

## ✔️ 1. Clone the Repository
```bash
git clone https://github.com/sadikshaik01/JobPortel.git
cd JobPortel


Create MySQL Database
CREATE DATABASE jobportel_db;

CREATE USER 'jobuser'@'localhost' IDENTIFIED BY 'jobpass';

GRANT ALL PRIVILEGES ON jobportel_db.* TO 'jobuser'@'localhost';
FLUSH PRIVILEGES;


## 🔧 Backend Setup (Spring Boot)
Navigate to backend folder:
cd JobPortal/JobPortal

Configure application.properties:
spring.datasource.url=jdbc:mysql://localhost:3306/jobportel_db
spring.datasource.username=jobuser
spring.datasource.password=jobpass

spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=true
spring.jpa.database-platform=org.hibernate.dialect.MySQL8Dialect

server.port=8080

Run backend (Maven):
./mvnw spring-boot:run


or

mvn spring-boot:run


Backend will run at:
👉 http://localhost:8080

💻 Frontend Setup (React + Vite)
Navigate:
cd "jobportal frontend/jobportal"

Install Dependencies:
npm install

Create .env file:
VITE_API_BASE_URL=http://localhost:8080

Run Dev Server:
npm run dev
