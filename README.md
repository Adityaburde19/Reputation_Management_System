# Reputation Management System - Backend

A modern Python backend application built with FastAPI for managing reputation systems. This project provides a robust, scalable, and well-structured API backend with comprehensive functionality for reputation management.

## 🚀 Project Overview

This is a FastAPI-based backend service designed for reputation management systems. The application follows modern Python development practices with a modular architecture, making it easy to maintain and scale.

### Key Features

- **FastAPI Framework**: High-performance, modern web framework for building APIs
- **Modular Architecture**: Well-organized code structure with clear separation of concerns
- **CORS Support**: Cross-Origin Resource Sharing enabled for frontend integration
- **Environment Configuration**: Flexible environment-based configuration
- **Auto-documentation**: Built-in API documentation with Swagger/ReDoc
- **Poetry Dependency Management**: Modern Python dependency and package management

## 📁 Current Project Structure

```
python-main-backend/
├── .env                    # Environment variables
├── poetry.lock            # Poetry dependency lock file
├── pyproject.toml         # Poetry project configuration
├── README.md              # Project documentation
├── server.py              # Main server entry point
├── doc/                   # Documentation
│   └── FOLDER_STRUCTURE.md
├── public/                # Public assets
├── src/                   # Source code
│   ├── app.py             # Main FastAPI application
│   ├── apis/              # API modules
│   ├── constants/         # Application constants
│   ├── controllers/       # Request controllers
│   ├── database/          # Database related files
│   ├── environment/       # Environment configuration
│   ├── helpers/           # Helper functions
│   ├── middlewares/       # Middleware functions
│   ├── models/            # Data models
│   ├── routes/            # Route definitions
│   ├── services/          # Business logic services
│   ├── types/             # Type definitions
│   └── utils/             # Utility functions
└── __pycache__/           # Python cache files
```

## 🛠️ Current Libraries

- **Python**: >= 3.10
- **FastAPI**: 0.116.1 - Modern, fast web framework
- **Uvicorn**: ASGI server for running the application
- **Pydantic**: Data validation and settings management
- **Requests**: HTTP library for making API calls
- **Python-dotenv**: Environment variable management

## 📋 Prerequisites

Before setting up the project, ensure you have the following installed:

- **Python 3.10 or higher**
- **Poetry** (Python dependency management tool)
- **Git** (for version control)

### Installing Poetry

If you don't have Poetry installed, install it using one of these methods:

**Windows (PowerShell):**
```powershell
(Invoke-WebRequest -Uri https://install.python-poetry.org -UseBasicParsing).Content | py -
```

**macOS/Linux:**
```bash
curl -sSL https://install.python-poetry.org | python3 -
```

## 🚀 Setup Instructions

### 1. Clone the Repository

```bash
git clone <repository-url>
cd python-main-backend
```

### 2. Install Dependencies

```bash
poetry install
```

This will create a virtual environment and install all required dependencies.

### 3. Environment Configuration

Create a `.env` file in the root directory with the following variables:

```env
# Server Configuration
HOST=0.0.0.0
PORT=6060
ENVIRONMENT=development

# Add other environment variables as needed
# DATABASE_URL=your_database_url
# SECRET_KEY=your_secret_key
# API_KEY=your_api_keys
```

### 4. Activate Virtual Environment

```bash
poetry shell
```

## 🏃‍♂️ Running the Application

### Development Mode

To run the application in development mode with auto-reload:

```bash
poetry run start
```

Or if you're in the Poetry shell:

```bash
python server.py
```

### Alternative Running Methods

**Using Poetry directly:**
```bash
poetry run python server.py
```

**Using Uvicorn directly:**
```bash
poetry run uvicorn src.app:app --host 0.0.0.0 --port 6060 --reload
```

## 📖 API Documentation

Once the server is running, you can access the API documentation at:

- **Swagger UI**: `http://localhost:6060/docs`
- **ReDoc**: `http://localhost:6060/redoc`
- **Health Check**: `http://localhost:6060/public/health-check`

## 🧪 Development

### Adding New Dependencies

To add new dependencies to the project:

```bash
poetry add package-name
```

For development dependencies:

```bash
poetry add --group dev package-name
```

### Project Scripts

The project includes a custom script defined in `pyproject.toml`:

- `poetry run start`: Starts the development server

### Code Organization

- **`src/app.py`**: Main FastAPI application with middleware configuration
- **`src/routes/`**: API route definitions
- **`src/controllers/`**: Request handling logic
- **`src/services/`**: Business logic layer
- **`src/models/`**: Data models and schemas
- **`src/database/`**: Database configuration and schemas
- **`src/middlewares/`**: Custom middleware functions
- **`src/helpers/`**: Helper functions and utilities
- **`src/environment/`**: Environment configuration management

## 🐛 Troubleshooting

### Common Issues

1. **Port already in use**: Change the PORT in your `.env` file
2. **Poetry not found**: Ensure Poetry is installed and added to your PATH
3. **Python version issues**: Ensure you have Python 3.10 or higher installed

### Useful Commands

```bash
# Check Poetry version
poetry --version

# Show current environment info
poetry env info

# List installed packages
poetry show

# Update dependencies
poetry update

# Check for security vulnerabilities
poetry audit
```

## 📞 Support

For support and questions, please contact the development team or create an issue in the repository.
Contact - Aditya Burde
