# Django Student API

A simple student management API built during today's Django REST Framework class.

## What We Covered

- Creating a Django project and application
- Defining a `Student` model
- Creating a model serializer
- Building function-based API views
- Adding URL routes
- Creating database migrations
- Supporting `GET`, `POST`, `PUT`, and `DELETE` requests

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

```bash
python manage.py migrate
python manage.py runserver
```

The API is available at `http://127.0.0.1:8000/api/students/`.
