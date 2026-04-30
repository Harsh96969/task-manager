# 🚀 Team Task Manager (Full Stack MERN App)

## 📌 Overview

This is a **Full Stack Team Task Manager Web Application** where users can create projects, assign tasks, and track progress with **role-based access control (Admin/Member)**.

The application is built using the **MERN Stack (MongoDB, Express, React, Node.js)** and deployed on **Railway**.

---

## 🛠️ Tech Stack Used

### 🔹 Backend

* **Node.js** – Runtime environment
* **Express.js** – REST API framework
* **MongoDB (Atlas)** – NoSQL database
* **Mongoose** – ODM for MongoDB
* **JWT (jsonwebtoken)** – Authentication
* **bcryptjs** – Password hashing
* **dotenv** – Environment variable management
* **cors** – Cross-origin requests handling

---

### 🔹 Frontend

* **React.js** – UI development
* **Vite** – Fast frontend build tool
* **Axios** – API requests handling

---

### 🔹 Deployment

* **Railway** – Backend deployment
* **MongoDB Atlas** – Cloud database

---

## 🔐 Features

### ✅ Authentication

* User Signup & Login
* Secure password hashing (bcrypt)
* JWT-based authentication

---

### 📁 Project Management

* Admin can create projects
* Projects can include multiple members
* Relationship maintained using MongoDB references

---

### 📌 Task Management

* Create and assign tasks
* Task status tracking:

  * Todo
  * In Progress
  * Done
* Tasks linked with users and projects

---

### 📊 Dashboard

* Total tasks count
* Completed tasks count
* Overdue tasks tracking (based on due date)

---

### 🔒 Role-Based Access Control

* **Admin**

  * Can create projects
* **Member**

  * Can view and work on assigned tasks

---

## 🧱 Project Structure

```
task-manager/
│
├── backend/
│   ├── models/
│   ├── routes/
│   ├── middleware/
│   ├── server.js
│   └── .env
│
├── frontend/
│   ├── src/
│   └── index.html
```

---

## ⚙️ How It Works

### 🔹 Backend Flow

1. User registers → password is hashed using bcrypt
2. User logs in → JWT token generated
3. Token is used to access protected routes
4. Middleware verifies user role (Admin/Member)
5. Data stored and managed using MongoDB

---

### 🔹 Database Relationships

* User → Projects (Members)
* Project → Tasks
* Task → Assigned User

---

## ▶️ Run Locally

### Backend

```
cd backend
npm install
npm start
```

### Frontend

```
cd frontend
npm install
npm run dev
```

---

## 🌍 Environment Variables

Create `.env` file in backend:

```
MONGO_URI=your_mongodb_connection
JWT_SECRET=your_secret_key
```

---

## 🚀 Deployment

* Code pushed to GitHub
* Connected GitHub repo to Railway
* Backend deployed using Railway
* MongoDB Atlas used as database

---

## 📹 Demo

* Signup / Login
* Create Project (Admin)
* Create Task
* Assign Task
* View Dashboard

---

## 🎯 Conclusion

This project demonstrates:

* Full Stack Development (MERN)
* REST API design
* Authentication & Authorization
* Database relationships
* Deployment on cloud

---

## 👨‍💻 Author

Harsh Kumar

---
@AGENTS.md
