---

## Getting Started

### Prerequisites
- Python 3.13
- pip or uv

### Installation

```bash
# Clone the repository
git clone https://github.com/faizan102418/finance-tracker-api.git
cd finance-tracker-api

# Install dependencies
pip install -r requirements.txt

# Run migrations
python manage.py migrate

# Start the server
python manage.py runserver
```

The API will be running at `http://127.0.0.1:8000/`

---

## API Endpoints

| Method | Endpoint | Description |
|--------|----------|-------------|
| GET | `/api/transactions/` | List all transactions |
| POST | `/api/transactions/` | Create a new transaction |
| GET | `/api/transactions/{id}/` | Get a single transaction |
| PUT | `/api/transactions/{id}/` | Update a transaction |
| DELETE | `/api/transactions/{id}/` | Delete a transaction |

---

## Testing with Postman

You can test all endpoints using Postman:

1. Start the server with `python manage.py runserver`
2. Open Postman
3. Send a GET request to `http://127.0.0.1:8000/api/transactions/`
4. Send a POST request with a JSON body to create a transaction

Example POST body:
```json
{
  "title": "Freelance Payment",
  "amount": 500.00,
  "category": "income"
}
```

---

## Status

Currently in active development as part of the Meta Backend Development Professional Certificate (Coursera). Features being added as new concepts are learned.

Planned additions:
- Token-based authentication
- Filtering and search
- Deployment on Railway or Render

---

## Author

**Muhammad Faizan Sajid**
- LinkedIn: [linkedin.com/in/faizan102418](https://linkedin.com/in/faizan102418)
- GitHub: [@faizan102418](https://github.com/faizan102418)

---

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.