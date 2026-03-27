# ⚙️ Node REST API (TypeScript + Express + MongoDB)


<div align="center">
  <img src="https://img.shields.io/badge/-TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white" alt="TypeScript" />
  <img src="https://img.shields.io/badge/-Node.js-339933?style=for-the-badge&logo=node.js&logoColor=white" alt="Node.js" />
  <img src="https://img.shields.io/badge/-Express.js-000000?style=for-the-badge&logo=express&logoColor=white" alt="Express.js" />
  <img src="https://img.shields.io/badge/-MongoDB-47A248?style=for-the-badge&logo=mongodb&logoColor=white" alt="MongoDB + Mongoose" />
  <img src="https://img.shields.io/badge/-JWT-000000?style=for-the-badge&logo=jsonwebtokens&logoColor=white" alt="JWT (Authentication)" />
  <img src="https://img.shields.io/badge/-argon2-003366?style=for-the-badge&logo=security&logoColor=white" alt="argon2" />
  <img src="https://img.shields.io/badge/-dotenv-009639?style=for-the-badge&logo=dotenv&logoColor=white" alt="dotenv" />
  <img src="https://img.shields.io/badge/-Joi-FFB703?style=for-the-badge&logo=javascript&logoColor=black" alt="Joi Validation" />
  <a href="https://node-mongoose-jwt-apis.onrender.com" target="_blank">


</div>


---

## 🧭 Table of Contents

- [📖 Introduction](#-introduction)
- [⚙ Tech Stack](#-tech-stack)
- [🔋 Features](#-features)
- [📦 Quick Start](#-quick-start)
- [🚀 Deployment on Render](#-deployment-on-render)
- [🧱 API Modules Overview](#-api-modules-overview)


---

## 📖 Introduction

This project is a **TypeScript-based REST API boilerplate** for scalable backend development.  
It provides fully functional modules for **Authentication**, **User Management**, **Products**, and **Students**.

Cleanly structured, type-safe, and production-ready.

---

## ⚙ Tech Stack

| Technology | Purpose |
|-------------|----------|
| **Node.js** | JavaScript runtime |
| **TypeScript** | Static typing for maintainable code |
| **Express.js** | Web framework for building APIs |
| **MongoDB + Mongoose** | NoSQL database and ODM |
| **JWT** | Authentication and authorization |
| **Joi** | Request validation |
| **dotenv** | Environment configuration |
| **ESLint + Prettier** | Linting and formatting |
| **tsx** | TypeScript runtime for development |

---

## 🔋 Features

✅ **JWT-based Authentication**  
✅ **Role-based Access (Admin / User)**  
✅ **CRUD APIs for Users, Products, and Students**  
✅ **Validation using Joi**  
✅ **Centralized Error Handling**  
✅ **TypeScript + Mongoose Models**  
✅ **Environment Configuration via .env**  
✅ **Clean Folder Structure**

---

## 📦 Quick Start

### 1️⃣ Clone the repository
```bash
git clone https://github.com/aswinsivadas-tech/node-rest-api-typescript.git
cd node-rest-api-typescript
```
### 2️⃣ Install Dependencies
```bash
npm install
```
## 3️⃣ Environment Variables (.env)

Create a `.env` file in the root of your project and add the following:

```env
# Server Port
PORT=5000

# MongoDB Connection URI
MONGO_URI=mongodb+srv://<USERNAME>:<PASSWORD>@<CLUSTER>.mongodb.net/

# MongoDB Database Name
MONGO_DB_NAME=<DATABASE_NAME>

# JWT Secret Key for Authentication
JWT_SECRET=<YOUR_JWT_SECRET_KEY>

# Node Environment
NODE_ENV=development
```
### 4️⃣ Start the server
```bash
npm run dev      # Development mode (with tsx watch)
npm run build    # Build TypeScript to dist/
npm start        # Run production build
```

---
Server will run on:  
👉 **http://localhost:3000**


---

## 🧱 API Modules Overview

### 🔐 Auth Routes — `/api/auth`
| Method | Endpoint | Description |
|--------|-----------|-------------|
| `POST` | `/register` | Register a new user |
| `POST` | `/login` | Login and receive JWT token |

---

### 👤 User Routes — `/api/users`
| Method | Endpoint | Description |
|--------|-----------|-------------|
| `GET` | `/` | Get all users |
| `GET` | `/:id` | Get single user by ID |

---

### 📦 Product Routes — `/api/products`
| Method | Endpoint | Description |
|--------|-----------|-------------|
| `POST` | `/` | Add new product (Admin only) |
| `GET` | `/` | Get all products (User access) |
| `PATCH` | `/:id` | Update product (Admin only) |
| `DELETE` | `/:id` | Delete product (Admin only) |

---

### 🎓 Student Routes — `/api/students`
| Method | Endpoint | Description |
|--------|-----------|-------------|
| `POST` | `/` | Add a new student |
| `GET` | `/` | Get all students |
| `GET` | `/:id/marks` | Get specific student’s marks |
| `PATCH` | `/:id` | Update student details |
| `DELETE` | `/:id` | Delete student record |
---
## 🧑‍💻 Scripts

| Command | Description |
|----------|--------------|
| `npm run dev` | Start development server with watch mode |
| `npm run build` | Compile TypeScript files |
| `npm start` | Run compiled app (production) |
| `npm run lint` | Lint all TypeScript files |
| `npm run lint:fix` | Fix lint errors automatically |
| `npm run format` | Format code with Prettier |


If you like this project, **please ⭐ star the repo!**