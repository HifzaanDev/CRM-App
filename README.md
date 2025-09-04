# 🚀 Django CRM Application

![Django](https://img.shields.io/badge/Django-4.1-green?style=for-the-badge&logo=django)
![Python](https://img.shields.io/badge/Python-3.x-blue?style=for-the-badge&logo=python)
![MySQL](https://img.shields.io/badge/MySQL-8.0-orange?style=for-the-badge&logo=mysql)
![Bootstrap](https://img.shields.io/badge/Bootstrap-5.0-purple?style=for-the-badge&logo=bootstrap)

A modern, feature-rich Customer Relationship Management (CRM) system built with Django. This application provides comprehensive customer data management with an intuitive web interface, user authentication, and full CRUD operations.

## 📋 Table of Contents

- [🌟 Features](#-features)
- [🏗️ Project Structure](#️-project-structure)
- [🔧 Installation](#-installation)
- [🚀 Quick Start](#-quick-start)
- [📖 Usage](#-usage)
- [🔒 Authentication](#-authentication)
- [🖼️ Screenshots](#️-screenshots)
- [🛠️ Technologies Used](#️-technologies-used)
- [🤝 Contributing](#-contributing)
- [📝 License](#-license)
- [👤 Author](#-author)

## 🌟 Features

✅ **User Authentication System**
- User registration and login
- Session management
- Password validation and security

✅ **Customer Management**
- Add new customer records
- View customer details
- Update existing records
- Delete customer records
- Comprehensive customer information storage

✅ **Responsive Design**
- Bootstrap 5 integration
- Mobile-friendly interface
- Clean and modern UI

✅ **Database Integration**
- MySQL database support
- Django ORM for data management
- Secure data storage

✅ **Form Validation**
- Client-side and server-side validation
- Error handling and user feedback
- Input sanitization

## 🏗️ Project Structure

```
CRM-App/
│
├── 📁 dcrm/                    # Django project configuration
│   ├── __init__.py
│   ├── asgi.py                 # ASGI configuration
│   ├── settings.py             # Project settings
│   ├── urls.py                 # Main URL configuration
│   └── wsgi.py                 # WSGI configuration
│
├── 📁 website/                 # Main application
│   ├── 📁 migrations/          # Database migrations
│   │   ├── 0001_initial.py
│   │   └── __init__.py
│   │
│   ├── 📁 templates/           # HTML templates
│   │   ├── add_record.html     # Add customer form
│   │   ├── base.html           # Base template
│   │   ├── home.html           # Dashboard/home page
│   │   ├── navbar.html         # Navigation component
│   │   ├── record.html         # Customer detail view
│   │   ├── register.html       # User registration
│   │   └── update_record.html  # Update customer form
│   │
│   ├── __init__.py
│   ├── admin.py                # Django admin configuration
│   ├── apps.py                 # App configuration
│   ├── forms.py                # Form definitions
│   ├── models.py               # Database models
│   ├── tests.py                # Unit tests
│   ├── urls.py                 # App URL patterns
│   └── views.py                # View functions
│
├── .gitignore                  # Git ignore rules
├── manage.py                   # Django management script
├── mydb.py                     # Database setup script
└── README.md                   # Project documentation
```

## 🔧 Installation

### Prerequisites

- Python 3.8+ installed on your system
- MySQL server (8.0+ recommended)
- pip (Python package manager)

### Step 1: Clone the Repository

```bash
git clone https://github.com/HifzaanDev/CRM-App.git
cd CRM-App
```

### Step 2: Create Virtual Environment (Recommended)

```bash
# Windows
python -m venv venv
venv\Scripts\activate

# macOS/Linux
python3 -m venv venv
source venv/bin/activate
```

### Step 3: Install Dependencies

```bash
pip install django
pip install mysql-connector-python
```

### Step 4: Database Setup

#### Option A: MySQL Setup
1. Install MySQL from [official website](https://dev.mysql.com/downloads/installer/)
2. Create database:
```bash
python mydb.py
```

#### Option B: SQLite (Development)
Modify `settings.py` to use SQLite:
```python
DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.sqlite3',
        'NAME': BASE_DIR / 'db.sqlite3',
    }
}
```

### Step 5: Run Migrations

```bash
python manage.py makemigrations
python manage.py migrate
```

### Step 6: Create Superuser

```bash
python manage.py createsuperuser
```

## 🚀 Quick Start

1. **Start the development server:**
```bash
python manage.py runserver
```

2. **Access the application:**
   - Main application: http://127.0.0.1:8000/
   - Admin panel: http://127.0.0.1:8000/admin/

3. **Create your first user account** through the registration page

4. **Start managing customers** by adding new records

## 📖 Usage

### 🏠 Dashboard
- View all customer records in a clean table format
- Quick access to customer actions (View, Edit, Delete)
- User authentication status and navigation

### 👤 Customer Management
- **Add Customer**: Fill out the comprehensive form with customer details
- **View Customer**: See detailed customer information
- **Edit Customer**: Update existing customer records
- **Delete Customer**: Remove customers from the system

### 🔐 User Management
- **Register**: Create new user accounts
- **Login**: Secure authentication system
- **Logout**: Session management

## 🔒 Authentication

The application includes a robust authentication system:
- User registration with form validation
- Secure login/logout functionality
- Session-based authentication
- Protected routes requiring authentication
- Password validation and security measures

## 🖼️ Screenshots

### Dashboard
The main dashboard displays all customer records with easy navigation and management options.

### Customer Details
Detailed view of individual customer information with edit and delete options.

### User Registration
Clean and user-friendly registration form with validation.

## 🛠️ Technologies Used

### Backend
- **Django 4.1** - Python web framework
- **Python 3.x** - Programming language
- **MySQL** - Database management system

### Frontend
- **HTML5** - Markup language
- **CSS3** - Styling
- **Bootstrap 5** - CSS framework
- **JavaScript** - Client-side scripting

### Tools & Libraries
- **Django ORM** - Object-relational mapping
- **MySQL Connector** - Database connectivity
- **Django Forms** - Form handling and validation

## 🤝 Contributing

Contributions are welcome! Here's how you can help:

1. **Fork the repository**
2. **Create a feature branch** (`git checkout -b feature/AmazingFeature`)
3. **Commit your changes** (`git commit -m 'Add some AmazingFeature'`)
4. **Push to the branch** (`git push origin feature/AmazingFeature`)
5. **Open a Pull Request**

### Development Guidelines
- Follow PEP 8 style guidelines
- Add comments for complex logic
- Update tests for new features
- Update documentation as needed

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 👤 Author

**Hifzaan Mohammad**

- 🌐 **GitHub**: [@HifzaanDev](https://github.com/HifzaanDev)
- 💼 **LinkedIn**: [Hifzaan Mohammad](https://www.linkedin.com/in/hifzaan-mohammad/)
- 📧 **Email**: Contact via LinkedIn

---

### 🌟 Show your support

Give a ⭐️ if this project helped you!

### 📈 Future Enhancements

- 📊 Customer analytics dashboard
- 📧 Email integration
- 📱 Mobile application
- 🔄 API development
- 📋 Export/Import functionality
- 🔍 Advanced search and filtering
- 📈 Sales tracking and reporting

---

*Built with ❤️ using Django and Python*
