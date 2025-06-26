# Clinic Appointment API

A RESTful API for managing clinic appointments built using **Django REST Framework**, **JWT Authentication**, and **MySQL**. This system allows different users (Admin, Doctor, Patient) to register, login, and manage appointment bookings securely.

---

## Features

-  JWT Authentication for secure login/logout.
-  Role-based permissions: Admin, Doctor, Patient.
-  Patients can book available appointments with doctors.
-  Doctors can view their appointments.
-  Permissions enforced at API level.
-  Filtering and pagination support.
- Swagger documentation included.

---

## 🛠️ Technologies Used

- Python 3.11+
- Django 4.x
- Django REST Framework
- SimpleJWT
- MySQL
- django-filter
- drf-yasg (Swagger UI)

---

##  Project Structure
clinic_project/
├── clinic/ # Main app (models, views, serializers, urls)
├── clinic_project/ # Project settings and configuration
├── filters.py # Custom filters
├── permissions.py # Custom permissions
├── manage.py
└── requirements.txt
---
# Roles and Permissions
Role	Capabilities
Admin	Full access to all resources
Doctor	View own appointments
Patient	Book and view their own appointments only
---
# Endpoints Overview
Examples:

/api/token/ - Obtain JWT token

/api/token/refresh/ - Refresh token

/api/appointments/ - List, Create, Manage appointments

/api/doctors/ - View doctor data

/api/patients/ - View patient data

