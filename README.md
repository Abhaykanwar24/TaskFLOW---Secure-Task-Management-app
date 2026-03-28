# TaskFLOW - Secure Task Management App 📝🔒

![Python](https://img.shields.io/badge/Python-3.14+-3776AB?style=for-the-badge&logo=python&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-005571?style=for-the-badge&logo=fastapi)
![SQLite](https://img.shields.io/badge/SQLite-07405E?style=for-the-badge&logo=sqlite&logoColor=white)
![Bootstrap](https://img.shields.io/badge/Bootstrap-563D7C?style=for-the-badge&logo=bootstrap&logoColor=white)

**TaskFLOW** is a modern, secure, and efficient web-based task management application built with **FastAPI** and **Python**. It offers a full-stack solution with server-side rendering using Jinja2 templates, ensuring a fast and responsive user experience. Included are robust authentication mechanisms, role-based access control, and a clean user interface.

## 🚀 Features

-   **🔐 Secure Authentication**: Full user registration and login system using **OAuth2** with **JWT** tokens.
-   **🛡️ Robust Security**: Passwords are securely hashed using **Argon2**, the industry standard for password hashing.
-   **✅ Task Management**: Create, Read, Update, and Delete (CRUD) personal todos.
-   **📊 Priority System**: Assign priority levels to tasks to stay organized.
-   **👤 User Profile**: Update personal details, change passwords, and manage phone numbers.
-   **👑 Admin Dashboard**: Special admin privileges to view and manage all users' tasks.
-   **📱 Responsive Design**: Built with Bootstrap to work seamlessly on desktop and mobile.

## 🛠️ Tech Stack

-   **Backend**: Python 3.14+, FastAPI, Starlette
-   **Database**: SQLite (SQLAlchemy ORM)
-   **Frontend**: HTML5, CSS3, JavaScript, Jinja2 Templates, Bootstrap 4/5
-   **Security**: Python-Jose (JWT), Passlib (Argon2), BCrypt (Legacy support)
-   **Testing**: Pytest

## ⚙️ Installation & Setup

Follow these steps to get the project running on your local machine.

### 1. Clone the Repository
```bash
git clone https://github.com/Abhaykanwar24/TaskFLOW---Secure-Task-Management-app.git
cd TaskFLOW---Secure-Task-Management-app
```

### 2. Create a Virtual Environment
It is recommended to use a virtual environment to manage dependencies.
```bash
# Windows
python -m venv .venv
.\.venv\Scripts\activate

# macOS/Linux
python3 -m venv .venv
source .venv/bin/activate
```

### 3. Install Dependencies
```bash
pip install -r requirements.txt
```

### 4. Run the Application
Start the development server using Uvicorn.
```bash
uvicorn main:app --reload
```
The application will be available at imports `http://127.0.0.1:8000`.

## 📖 Usage

1.  **Register**: Create a new account at `/auth/register-page`.
2.  **Login**: Log in with your credentials at `/auth/login-page`.
3.  **Manage Todos**: Access your dashboard to add, edit, or complete tasks.
4.  **Admin**: If you have an admin account, access `/admin/todo` to oversee all activities.

## 🧪 Running Tests

This project includes a comprehensive test suite. To run the tests:

```bash
pytest
```

## 📂 Project Structure

```
TodoApp/
├── .venv/                   # Virtual Environment
├── alembic/                 # Database Migrations
├── routers/                 # API Routes (Auth, Todos, Users, Admin)
├── static/                  # CSS, JS, Images
├── templates/               # HTML Templates (Jinja2)
├── test/                    # Unit & Integration Tests
├── main.py                  # Application Entry Point
├── models.py                # Database Models
├── database.py              # Database Connection
├── requirements.txt         # Project Dependencies
└── README.md                # Project Documentation
```


