# Support System Backend

A backend REST API built using Django and Django REST Framework for managing users, services, and support tickets.

---

## Features
- Custom User model
- Role-based authentication & authorization
- Ticket creation and management
- Service mapping
- PostgreSQL database
- REST APIs using DRF

---

## 🛠 Tech Stack
- Python
- Django
- Django REST Framework
- PostgreSQL
- pgAdmin
- python-dotenv

---

## 📁 Project Structure
```
task/
├── manage.py
├── .env
├── .gitignore
├── requirements.txt
├── users/
├── core/
├── support/
├── myproject/
└── venv/
```


---

## ⚙️ Setup Instructions

1️⃣ Clone the repository
```
git clone <your-repo-url>
cd task
```

2️⃣ Create virtual environment
```
python -m venv venv
venv\Scripts\activate   # Windows
```

3️⃣ Install dependencies
```
pip install -r requirements.txt
```
4️⃣ Environment variables

Create a .env file in the project root:

SECRET_KEY=your-secret-key
DEBUG=True

DB_NAME=support_system
DB_USER=postgres
DB_PASSWORD=yourpassword
DB_HOST=localhost
DB_PORT=5432

5️⃣ Run migrations
```
python manage.py makemigrations
python manage.py migrate
```

6️⃣ Start development server
```
python manage.py runserver
```

Server runs at:
```
http://127.0.0.1:8000/
```

🔌 API Testing

You can test APIs using:

Thunder Client

Postman

Example:
```
GET /api/support/tickets/
```
