# Mini JIRA - Bug Tracker API

A **Mini JIRA clone** built using Django and Django REST Framework.  
This is a full-featured backend for tracking issues with priorities, statuses, and authenticated user actions.

> Frontend in progress using React  
> Docker + JWT + Cloud deployment coming soon

---

## Features

Built:
- Authenticated API (DRF + Django users)
- Create, update, delete issues
- Priority and status choices
- Reporter auto-assigned from logged-in user

Planned:
- JWT Authentication
- User roles: reporter / developer
- Projects & Issue grouping
- Comments on issues
- Filtering, search, and tags
- Docker and deployment to Render

---

## Tech Stack

- Python 3.13
- Django 5.2
- Django REST Framework
- SQLite (dev DB)
- React (upcoming frontend)
- Docker (coming soon)

---

## API Endpoints

| Method | URL                   | Description              |
|--------|------------------------|--------------------------|
| POST   | `/api/issues/`         | Create issue             |
| GET    | `/api/issues/`         | List all user issues     |
| GET    | `/api/issues/<id>/`    | Get issue details        |
| PUT    | `/api/issues/<id>/`    | Update issue             |
| DELETE | `/api/issues/<id>/`    | Delete issue             |

> All endpoints require login (basic/session auth)

---

## Setup

```bash
git clone https://github.com/yourusername/bugtracker-backend.git
cd bugtracker-backend
python -m venv env
source env/bin/activate
pip install -r requirements.txt
python manage.py migrate
python manage.py createsuperuser
python manage.py runserver


## Author

**Avanti Deshpande**  
Python Full Stack Developer | Django | Flask | FastAPI | Angular | React | Learning AI  
