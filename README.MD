# FastAPI Issue Tracker

A simple issue-tracking REST API built with FastAPI while learning modern Python API development.

The project explores how to structure a FastAPI application, define data schemas, organize endpoints with routers, manage issue data, and use middleware.

## Features

- REST API endpoints for managing issues
- Request and response validation using Pydantic schemas
- Organized route handling with FastAPI routers
- JSON-based data storage
- Custom middleware for request timing
- Interactive API documentation with Swagger UI

## Tech Stack

- Python
- FastAPI
- Pydantic
- Uvicorn
- JSON file storage

## Project Structure

```
fastapi-issue-tracker/
├── app/
│   ├── middleware/
│   │   └── timer.py
│   ├── routes/
│   │   └── issues.py
│   ├── schemas.py
│   └── storage.py
├── data/               # issues.json lives here (git-ignored)
├── main.py
├── requirements.txt
├── .gitignore
└── README.md
```

## Getting Started

### 1. Clone the repository

```
git clone https://github.com/D-Data-alchemist/fastapi-issue-tracker.git
cd fastapi-issue-tracker
```

### 2. Create a virtual environment

```
python -m venv .venv
```

Activate it on Windows PowerShell:

```
.venv\Scripts\Activate.ps1
```

On macOS/Linux:

```
source .venv/bin/activate
```

### 3. Install dependencies

```
pip install -r requirements.txt
```

### 4. Run the application

```
uvicorn main:app --reload --reload-exclude .venv
```

### 5. Explore the API

- Swagger UI: http://127.0.0.1:8000/docs
- ReDoc: http://127.0.0.1:8000/redoc

Issue endpoints live under `/api/v1/issues/`.

## What I Learned

- Building REST APIs with FastAPI
- Organizing code into routers and modules
- Defining schemas and validating requests
- Working with JSON-based storage
- Implementing middleware
- Reading auto-generated API documentation
- Debugging imports, virtual environments, and git setup

## Future Improvements

- Persist issues in a database (SQLite, then PostgreSQL)
- Add automated tests
- Add get-by-id, update, and delete endpoints
- Add authentication, pagination, and filtering
- Deploy to Render

## Project Status

A learning project built while following a FastAPI tutorial, and a foundation for further experimentation with backend development and API design.

## Author

Awwal Adepoju. Learning and building with Python, backend development, data engineering, and cloud technologies.