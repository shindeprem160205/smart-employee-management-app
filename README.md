

# Smart Employee & Office Management Mobile Application

A production-oriented employee and office management system designed as a mobile-first application with a Django REST API backend and PostgreSQL database.

The project is being developed with a focus on clean backend architecture, secure authentication, role-based access control, RESTful APIs, automated testing, containerization, and CI/CD.

---

## 🚧 Project Status

**Currently in active development.**

### Completed

- Django backend setup
- PostgreSQL database integration
- Custom Django User model
- Role-based user structure
- Django Admin configuration
- Superuser authentication
- Initial database migrations
- Git/GitHub project setup
- Python virtual environment
- Basic project configuration

### Planned

- JWT authentication
- Role-based API permissions
- Employee management
- Attendance management
- QR-based attendance
- Leave management
- Notifications
- Redis caching
- Celery background tasks
- Automated testing with Pytest
- Swagger/OpenAPI documentation
- React Native mobile application
- Docker and Docker Compose
- GitHub Actions CI/CD
- Cloud deployment

---

## 🎯 Project Objective

The objective of this project is to build a centralized mobile-based employee management platform that allows organizations to manage employees, attendance, leave requests, notifications, and administrative operations through a secure REST API and mobile application.

The system will support different user roles such as:

- **Admin**
- **HR**
- **Employee**

Each role will have access to functionality based on its permissions.

---

## 🏗️ Planned Architecture

```text
                 React Native Mobile App
                           |
                           | REST API
                           v
                 Django REST Framework
                           |
              +------------+------------+
              |                         |
              v                         v
        PostgreSQL                   Redis
              |                         |
              |                      Celery
              |                         |
              +------------+------------+
                           |
                    Background Tasks
