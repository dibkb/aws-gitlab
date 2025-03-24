# FastAPI Demo with Docker and Poetry

This is a boilerplate FastAPI application using Docker and Poetry for dependency management.

## Prerequisites

- Docker and Docker Compose
- Poetry (optional, for local development)

## Getting Started

### Using Docker Compose (Recommended)

1. Build and start the application:

```bash
docker-compose up --build
```

2. The API will be available at http://localhost:8000

3. API documentation will be available at:
   - Swagger UI: http://localhost:8000/docs
   - ReDoc: http://localhost:8000/redoc

### Local Development

1. Install dependencies:

```bash
poetry install
```

2. Run the application:

```bash
poetry run uvicorn app.main:app --reload
```

## Available Endpoints

- `GET /`: Welcome message
- `GET /health`: Health check endpoint

## Development

- The application uses Poetry for dependency management
- Code formatting is handled by Black
- Import sorting is handled by isort
- Linting is handled by flake8

## License

MIT
