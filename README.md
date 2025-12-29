# my_django_auth

A Django REST API authentication project using Django REST Framework, SimpleJWT, and dj-rest-auth.

## Features
- Token-based authentication (JWT)
- RESTful endpoints for login, logout, password reset, etc.
- Easily extensible for user registration and profile management

## Requirements
- Python 3.8+
- Django 5.x
- djangorestframework
- djangorestframework-simplejwt
- dj-rest-auth

## Setup

### 1. Clone the repository
```zsh
git clone https://github.com/aloba-james/my_django_auth.git
cd my_django_auth
```

### 2. Create and activate a virtual environment (if not already active)
```zsh
python3 -m venv .
source bin/activate
```

### 3. Install dependencies
```zsh
pip install --upgrade pip
pip install -r requirements.txt
```

### 4. Run migrations
```zsh
python manage.py migrate
```

### 5. Create a superuser (optional, for admin access)
```zsh
python manage.py createsuperuser
```

### 6. Start the development server
```zsh
python manage.py runserver
```

## API Endpoints
- `POST /api/v1/auth/login/` — Obtain JWT token
- `POST /api/v1/auth/logout/` — Logout
- `POST /api/v1/auth/password/reset/` — Password reset
- `POST /api/v1/auth/password/change/` — Change password

For more endpoints, see [dj-rest-auth documentation](https://dj-rest-auth.readthedocs.io/en/latest/api_endpoints.html).

## Project Structure
- `manage.py` — Django project management script
- `my_django_auth/` — Project settings and URLs
- `requirements.txt` — Python dependencies

## Notes
- The virtual environment is stored in the project root and is ignored by git.
- Default authentication endpoints are provided by dj-rest-auth and SimpleJWT.

## License
MIT
