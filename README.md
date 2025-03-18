# Bookstore - Django Project

## Overview
This is a Django-based Bookstore application that allows users to browse, search, and purchase books. Admins can manage books, categories, and orders through a dashboard.

## Features
- User Authentication (Signup/Login/Logout)
- Browse books by categories
- Search functionality
- Add books to cart
- Checkout and order management
- Admin panel for book and order management
- Responsive UI with Bootstrap/Tailwind

## Technologies Used
- **Backend:** Django, Django REST Framework
- **Frontend:** HTML, CSS, Bootstrap/Tailwind
- **Database:** SQLite/PostgreSQL
- **Deployment:** AWS/Heroku

## Installation Guide

### 1. Clone the Repository
```bash
git clone https://github.com/yourusername/bookstore.git
cd bookstore
```

### 2. Create a Virtual Environment
```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

### 3. Install Dependencies
```bash
pip install -r requirements.txt
```

### 4. Apply Migrations
```bash
python manage.py makemigrations
python manage.py migrate
```

### 5. Create Superuser (Admin Access)
```bash
python manage.py createsuperuser
```

### 6. Run the Server
```bash
python manage.py runserver
```
Access the application at `http://127.0.0.1:8000/`

## Project Structure
```
bookstore/
│── manage.py
│── requirements.txt
│── README.md
│── bookstore/  # Main Django project
│── books/      # Books app
│── users/      # User authentication
│── orders/     # Order management
│── templates/  # HTML templates
```

## API Endpoints (If using DRF)
| Method | Endpoint | Description |
|--------|----------|-------------|
| GET | /api/books/ | Get all books |
| POST | /api/books/ | Add a new book (Admin) |
| GET | /api/orders/ | Get user orders |

## Deployment
To deploy on Heroku:
```bash
git push heroku main
heroku run python manage.py migrate
```

## License
This project is licensed under the MIT License.

