# Finance Tracker API

A personal finance REST API built with Python & Django REST Framework.

## Features
- Track income and expenses
- Categorize transactions
- RESTful endpoints for full CRUD operations
- Token-based authentication

## Tech Stack
- Python 3.13
- Django & Django REST Framework
- SQLite (dev) / PostgreSQL (prod-ready)

## Getting Started

```bash
git clone https://github.com/faizan102418/finance-tracker-api.git
cd finance-tracker-api
pip install -r requirements.txt
python manage.py migrate
python manage.py runserver
```

## API Endpoints
| Method | Endpoint | Description |
|--------|----------|-------------|
| GET | /api/transactions/ | List all transactions |
| POST | /api/transactions/ | Create a transaction |
| GET | /api/transactions/{id}/ | Get a transaction |
| PUT | /api/transactions/{id}/ | Update a transaction |
| DELETE | /api/transactions/{id}/ | Delete a transaction |

## Author
Muhammad Faizan Sajid — [LinkedIn](https://www.linkedin.com/in/faizan102418)
