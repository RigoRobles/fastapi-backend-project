# English Learning Platform

A comprehensive web application for learning English, built with FastAPI and React.

## Features

- User Authentication (Login/Register)
- Student and Teacher Dashboards
- Interactive Lessons
- Progress Tracking
- Quiz System
- Real-time Statistics

## Tech Stack

### Frontend
- React with TypeScript
- Vite for build tooling
- TailwindCSS for styling
- React Router for navigation
- Axios for API requests
- React Query for state management

### Backend
- FastAPI (Python)
- SQLAlchemy for ORM
- Alembic for database migrations
- JWT for authentication
- PostgreSQL database

## Getting Started

### Prerequisites
- Node.js and npm
- Python 3.8+
- PostgreSQL

### Frontend Setup
```bash
cd frontend
npm install
npm run dev
```

### Backend Setup
```bash
# Create virtual environment
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt

# Set up environment variables
cp .env.example .env
# Edit .env with your configuration

# Run migrations
alembic upgrade head

# Start the server
python run.py
```

## Project Structure

```
.
├── frontend/               # React frontend
│   ├── src/
│   │   ├── components/    # Reusable components
│   │   ├── contexts/      # React contexts
│   │   ├── layouts/       # Layout components
│   │   ├── pages/         # Page components
│   │   ├── services/      # API services
│   │   └── types/         # TypeScript types
│   └── ...
│
└── backend/               # FastAPI backend
    ├── app/
    │   ├── api/          # API routes
    │   ├── core/         # Core functionality
    │   ├── models/       # Database models
    │   └── schemas/      # Pydantic schemas
    ├── alembic/          # Database migrations
    └── tests/            # Test suite
```

## API Documentation

Once the server is running, visit:
- Swagger UI: http://localhost:8000/docs
- ReDoc: http://localhost:8000/redoc

## Testing

Run the test suite:
```bash
pytest
```

## Contributing

1. Fork the repository
2. Create a feature branch
3. Commit your changes
4. Push to the branch
5. Create a Pull Request

## License

MIT License - see LICENSE file for details