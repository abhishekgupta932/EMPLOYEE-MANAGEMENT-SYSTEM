

# Employee Management System (EMS)

A simple full-stack Employee Management System built using **React (Vite)** for the frontend and **Spring Boot (Java 21)** for the backend.
Users can **add**, **update**, **list**, and **delete** employee records.

---

## 📸 Screenshots

**List Of Employee :**

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/31594c13-33a7-4ada-8ea7-4b9ab85807f9" />


**Add Employee :**

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/1c77045d-52fe-40f8-a60f-f414c4ce3625" />


**Update Employee :**

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/35e1003b-121b-4327-a632-1a88d017a59f" />

---

## 📝 Features

* Add New Employee
* Update Existing Employee
* Delete Employee
* Fetch Employee List
* Full REST API integration
* Simple and clean UI

---

## 🚀 Tech Stack

### **Frontend (React + Vite)**

* React 18
* React Router DOM
* Axios
* Vite
* Bootstrap version 5

### **Backend (Spring Boot)**

* Spring Web
* Spring Data JPA
* MySQL Driver
* Lombok

---

## 📂 Project Structure Overview

```
ems-frontend/
    src/
    package.json
    vite.config.js

ems-backend/
    src/
    pom.xml
```

---

# 🧩 Prerequisites

| Tool        | Version                                           |
| ----------- | ------------------------------------------------- |
| **Node.js** | 18+ recommended (your version: 24.15 is perfect)  |
| **npm**     | Comes with Node                                   |
| **Java**    | 21 or above                                       |
| **MySQL**   | 8+                                                |
| **IDE**     | IntelliJ IDEA (recommended) or Spring Tools Suite |

---

# 📦 Frontend Setup (React + Vite)

### **1. Open frontend project**

```
cd ems-frontend
```

### **2. Install dependencies**

```
npm install
```

This will create `node_modules` automatically based on your `package.json`.

### **3. Running the dev server**

```
npm run dev
```

Frontend runs on:
**[http://localhost:3000/](http://localhost:3000/)**

---

# 🧑‍💻 Backend Setup (Spring Boot)

### **1. Open project in IntelliJ**

File → Open → select **ems-backend**

### **2. Configure application.properties**

```
spring.datasource.url=jdbc:mysql://localhost:3306/employeeDB
spring.datasource.username=root
spring.datasource.password=yourPassword

spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=true
```

### **3. Build and Run**

Use IntelliJ:

* Click **Run → Run Application**
  OR

Terminal:

```
mvn spring-boot:run
```

Backend runs on:
**[http://localhost:8080](http://localhost:8080)**

---

# 🔗 API Endpoints (Backend)

| Method | Endpoint              | Description        |
| ------ | --------------------- | ------------------ |
| GET    | `/api/employees`      | Get all employees  |
| POST   | `/api/employees`      | Add employee       |
| GET    | `/api/employees/{id}` | Get employee by id |
| PUT    | `/api/employees/{id}` | Update employee    |
| DELETE | `/api/employees/{id}` | Delete employee    |

---

# ✔️ How Everything Connects

* React frontend calls Spring Boot API using **Axios**
* Spring Boot interacts with **MySQL** using **Spring Data JPA**
* Data flows back to React and updates UI

---

