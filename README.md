# Todo List App

![React](https://img.shields.io/badge/React-18-61DAFB?logo=react&logoColor=white)
![Django](https://img.shields.io/badge/Django-REST_API-092E20?logo=django&logoColor=white)
![Axios](https://img.shields.io/badge/Axios-HTTP_Client-5A29E4)
![License](https://img.shields.io/badge/License-MIT-green)

A beginner-friendly full-stack Todo List application built with **React** on the frontend and **Django REST Framework** on the backend. Manage your daily tasks with a clean, minimal interface.

---

## Features

- Add new tasks with a title and description
- Edit existing tasks via a popup modal
- Delete tasks with a single click
- Mark tasks as complete / incomplete
- Filter tasks by **All**, **Active**, or **Done**
- Optimistic UI updates — no page reload needed

---

## Tech Stack

### Frontend
- React (JSX)
- Axios — for HTTP requests
- CSS — custom styles with DM Sans font

### Backend
- Django — Python web framework
- Django REST Framework — API endpoints
- SQLite — default database (easily swappable)

---

## Getting Started

### Prerequisites
- Node.js & npm
- Python 3.x & pip

### Backend Setup

```bash
cd backend
pip install django djangorestframework
python manage.py migrate
python manage.py runserver
```

### Frontend Setup

```bash
cd frontend
npm install
npm start
```

The React app runs on `http://localhost:3000` and talks to the Django API at `http://127.0.0.1:8000`.

---

## API Endpoints

| Method | Endpoint | Description |
|--------|----------|-------------|
| GET | `/get_tasks/` | Fetch all tasks |
| POST | `/add_task/` | Add a new task |
| PUT | `/edit_task/<id>/` | Edit a task |
| DELETE | `/delete_task/<id>/` | Delete a task |

---

## Project Structure

```text
todo-app/
  frontend/
    src/
      Form.jsx        # Main component
      Form.css        # Styles
  backend/
    manage.py
    tasks/
      views.py        # API views
      models.py       # Task model
      urls.py         # URL routing
```

---

## License

This project is open source and available under the [MIT License](LICENSE).

---

*Built as a beginner project to learn React + Django full-stack development.*
