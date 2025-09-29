# <img src="https://cdn-icons-png.flaticon.com/512/18310/18310882.png" width="80"/> FastAPI Python Learning Repository
    
Welcome to the **FastAPI Python Learning Repository** — an interactive project that introduces Python concepts through [FastAPI](https://fastapi.tiangolo.com/), a modern web framework for building APIs with Python 3.7+.

---

## <img src="https://cdn-icons-png.flaticon.com/512/18310/18310957.png" width="80"/> What Is This?
   
This repository is both:
- A **learning resource** for Python, and  
- A **practical example** of building and serving content via **FastAPI**.

It transforms static educational content about Python into a dynamic API-powered web application.

---

## <img src="https://cdn-icons-png.flaticon.com/512/18310/18310909.png" width="80"/> Why FastAPI?

FastAPI is:
- ⚡ **Fast**: High-performance, powered by **Starlette** and **Pydantic**.  
- 🧑‍💻 **Beginner-friendly**: Minimal boilerplate, easy to get started.  
- 🔄 **Async-ready**: Native async support for modern Python.  
- 📚 **Well-documented**: Includes automatic Swagger and ReDoc docs.  

---

## <img src="https://cdn-icons-png.flaticon.com/512/7778/7778962.png" width="80"/> Setup

### 1. Clone the repository
```bash
git clone https://github.com/gil-son/fast-api.git
cd fast-api/
```

### 2. Create a virtual environment
```bash
python3 -m venv venv
```

### 3. Activate the environment
```bash
source venv/bin/activate
```

### 4. Install dependencies
```bash
pip install -r requirements.txt
```

### 5. About dependencies

This project relies on the following Python packages:

- **[fastapi](https://fastapi.tiangolo.com/)** – The core web framework used to build the API. Provides routing, request handling, validation, and automatic documentation (Swagger & ReDoc).
- **[uvicorn](https://www.uvicorn.org/)** – An ASGI server to run FastAPI applications in production or development mode. Required to serve the app.
- **[pytest](https://docs.pytest.org/)** – A testing framework that makes it easy to write and run unit tests for Python applications.
- **[pytest-cov](https://pytest-cov.readthedocs.io/)** – A pytest plugin that generates coverage reports, helping to ensure test completeness.
- **[taskipy](https://github.com/taskipy/taskipy)** – A simple task runner that allows you to define reusable commands (e.g., run, test, lint) in `pyproject.toml`.
- **[ruff](https://github.com/astral-sh/ruff)** – A fast Python linter and code formatter, ensuring code style consistency and catching errors early.

Together, these tools support development, testing, linting, formatting, and running the application smoothly.

### 6. Understanding `pyproject.toml`

Configured tasks:
```toml
[tool.taskipy.tasks]
lint = "ruff check"
pre_format = "ruff check --fix"
format = "ruff format"
run = "fastapi dev fast_zero/app.py"
pre_test = "task lint"
test = "pytest -s -x --cov=fast_zero -vv"
post_test = "coverage html"
```

### 7. Run the app
```bash
fastapi dev fast_zero/app.py
```

---

## <img src="https://cdn-icons-png.flaticon.com/512/18310/18310876.png" width="80"/> Repository Structure

```
fast-api/
├── fast_zero/
│   └── app.py           # Main FastAPI application
├── README.md            # Project documentation
└── requirements.txt     # Dependencies
```

---

## <img src="https://cdn-icons-png.flaticon.com/512/18310/18310796.png" width="80"/> References & Resources

- [Dunossauro - FastAPI do Zero](https://fastapidozero.dunossauro.com/estavel/)  
- [FastAPI Official Documentation](https://fastapi.tiangolo.com/)  

---
