# 🏥 Patient Management System API

A RESTful backend application built using **FastAPI** for efficient and scalable patient record management. The system provides complete CRUD functionality with robust request validation powered by **Pydantic**, ensuring clean data handling and reliable API behavior.

---

## 📌 Overview

The **Patient Management System API** is designed to streamline patient data operations in a structured and secure manner. It demonstrates backend best practices including:

* RESTful API architecture
* Data validation using Pydantic models
* Structured routing and modular design
* Automatic interactive API documentation
* Clean and scalable project structure

This project is ideal for showcasing backend development skills using FastAPI.

---

## 🚀 Features

* ✅ Create new patient records
* 📄 Retrieve individual or multiple patient records
* ✏️ Update existing patient details
* ❌ Delete patient records
* 🛡️ Data validation using Pydantic schemas
* 📘 Auto-generated API docs via Swagger UI

---

## 🛠️ Tech Stack

* **FastAPI** – High-performance web framework
* **Pydantic** – Data validation and serialization
* **Uvicorn** – ASGI server

---

## 📂 Project Structure

```
Patient-Management-System-API/
│
├── main.py                # Application entry point
├── patients.json          # DataSet
└── README.md
```

---

## ⚙️ Installation & Setup

### 1️⃣ Clone the Repository

```bash
git clone <your-repo-url>
cd Patient-Management-System-API
```

### 2️⃣ Create Virtual Environment (Recommended)

```bash
python -m venv venv
source venv/bin/activate   # For Mac/Linux
venv\Scripts\activate      # For Windows
```

### 3️⃣ Install Dependencies

```bash
pip install -r requirements.txt
```

### 4️⃣ Run the Application

```bash
uvicorn main:app --reload
```

---

## 🌐 API Documentation

Once the server is running, access interactive API documentation:

* Swagger UI:

  ```
  http://127.0.0.1:8000/docs
  ```

* ReDoc:

  ```
  http://127.0.0.1:8000/redoc
  ```

---

## 📌 Example Endpoints

| Method | Endpoint         | Description          |
| ------ | ---------------- | -------------------- |
| POST   | `/patients`      | Create a new patient |
| GET    | `/patients`      | Get all patients     |
| GET    | `/patients/{id}` | Get patient by ID    |
| PUT    | `/patients/{id}` | Update patient       |
| DELETE | `/patients/{id}` | Delete patient       |

---

## 🧠 Learning Objectives

This project demonstrates:

* Backend API design using FastAPI
* Input validation and schema enforcement
* Clean routing and modular architecture
* RESTful service implementation

