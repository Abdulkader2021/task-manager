# 📋 PM App — Project Management API

A simple project management backend built with **Node.js**, **Express**, **MongoDB**, and **JWT authentication**.  
Supports projects, tasks, status tracking, and self-assignment — designed as a learning project.

---

## ✨ Features

- 🔐 **Authentication**
  - Register / Login / Logout
  - JWT stored in **httpOnly cookies** (XSS-safe)
  - Protected routes via middleware

- 📁 **Projects**
  - Create, edit, delete, view
  - Owner-scoped queries (authorization enforced)

- ✅ **Tasks**
  - Create, edit, delete
  - Status: `todo` · `in-progress` · `done`
  - Assign task to yourself / unassign
  - Due dates
  - Cascade delete when project is removed

- 🛡️ **Security**
  - Password hashing with **bcryptjs**
  - Input validation with **Zod**
  - Ownership checks on every resource
  - Passwords never returned in responses

---

## 🧱 Tech Stack

| Layer      | Tech                          |
| ---------- | ----------------------------- |
| Runtime    | Node.js                       |
| Framework  | Express.js                    |
| Database   | MongoDB + Mongoose            |
| Auth       | JWT + httpOnly cookie         |
| Validation | Zod                           |
| Security   | bcryptjs, cors, cookie-parser |

---

## 📂 Project Structure
