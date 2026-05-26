# Finance Tracker API

![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)
![Django](https://img.shields.io/badge/Django-092E20?style=flat&logo=django&logoColor=white)
![DRF](https://img.shields.io/badge/Django_REST_Framework-ff1709?style=flat&logo=django&logoColor=white)
![License](https://img.shields.io/github/license/faizan102418/finance-tracker-api?style=flat)
![Last Commit](https://img.shields.io/github/last-commit/faizan102418/finance-tracker-api?style=flat&color=0e75b6)

A personal finance REST API built with Python and Django REST Framework. Track your income, expenses, and transactions through clean RESTful endpoints.

## Features

- Add, view, update and delete financial transactions
- Categorize transactions (income / expense)
- Filter transactions by category
- REST API endpoints tested with Postman
- Clean Django project structure with separated config and app modules

## Tech Stack

- Language: Python 3
- Framework: Django
- API: Django REST Framework
- Database: SQLite (development)
- Tools: Postman, Git, GitHub

## Project Structure
finance-tracker-api/
├── config/          # Project settings and URL configuration
├── tracker/         # Main app: models, views, serializers, URLs
├── manage.py        # Django management commands
├── pyproject.toml   # Project dependencies
└── .gitignore

## Getting Started

### Prerequisites

- Python 3.13
- pip or uv

### Installation

```bash
git clone https://github.com/faizan102418/finance-tracker-api.git
cd finance-tracker-api
pip install -r requirements.txt
python manage.py migrate
python manage.py runserver
```

The API will be running at http://127.0.0.1:8000/

## API Endpoints

- GET /api/transactions/ — List all transactions
- POST /api/transactions/ — Create a new transaction
- GET /api/transactions/{id}/ — Get a single transaction
- PUT /api/transactions/{id}/ — Update a transaction
- DELETE /api/transactions/{id}/ — Delete a transaction

## Testing with Postman

1. Start the server with `python manage.py runserver`
2. Open Postman
3. Send a GET request to `http://127.0.0.1:8000/api/transactions/`
4. Send a POST request with this JSON body:

```json
{
  "title": "Freelance Payment",
  "amount": 500.00,
  "category": "income"
}
```

## Status

Currently in active development as part of the Meta Backend Development Professional Certificate (Coursera). Features being added as new concepts are learned.

Planned additions:
- Token-based authentication
- Filtering and search
- Deployment on Railway or Render

## Author

Muhammad Faizan Sajid

- LinkedIn: [linkedin.com/in/faizan102418](https://linkedin.com/in/faizan102418)
- GitHub: [@faizan102418](https://github.com/faizan102418)

## License

This project is licensed under the MIT License. See the LICENSE file for details.
