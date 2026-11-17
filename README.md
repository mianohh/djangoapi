# Django Student API

A student management API built with Django and Django REST Framework. The
project provides CRUD operations for student records and uses MySQL for
persistent data storage.

## Student Model

Each student has:

- `name`
- `age`
- `email`

## API Endpoints

| Method | Endpoint | Description |
|---|---|---|
| GET | `/api/students/` | List all students |
| POST | `/api/students/` | Create a student |
| GET | `/api/students/<id>/` | Retrieve one student |
| PUT | `/api/students/<id>/` | Update a student |
| DELETE | `/api/students/<id>/` | Delete a student |

Example request body:

```json
{
  "name": "Jane Doe",
  "age": 20,
  "email": "jane@example.com"
}
```

## Run Locally

Configure the MySQL database connection in `djangoapi/settings.py`, then run:

```bash
python manage.py migrate
python manage.py runserver
```

The API is available at `http://127.0.0.1:8000/api/students/`.
