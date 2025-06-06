# 🚀 FastAPI Python Learning Repository

Welcome to the **FastAPI Python Learning Repository** — a simple, interactive web API that introduces Python concepts using [FastAPI](https://fastapi.tiangolo.com/), a modern web framework for building APIs with Python 3.7+.

## 🔧 What Is This?

This repository serves both as a:

- Learning resource for **Python beginners**, and
- Practical example of using **FastAPI** to build and serve content via an API.

It converts static educational content about Python into a dynamic web app using FastAPI.

## 🧠 Why FastAPI?

FastAPI is:
- **Fast**: High-performance, thanks to Starlette and Pydantic.
- **Easy to use**: Minimal boilerplate, great for beginners.
- **Async-ready**: Built on async support for modern Python.
- **Well-documented**: Comes with automatic Swagger docs out of the box.

## 📁 Project Structure

```
.
├── main.py         # FastAPI app with HTML response
├── README.md       # This file
└── requirements.txt  # (Optional) List of dependencies
```

## 🚀 How to Run It

### 1. Clone the repository

```bash
git clone https://github.com/gil-son/fast-api/.git
cd fast-api
```

### 2. Create a virtual environment (optional but recommended)

```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

### 3. Install FastAPI and Uvicorn

```bash
pip install fastapi uvicorn
```

### 4. Start the server

```bash
uvicorn main:app --reload
```

Then open [http://127.0.0.1:8000](http://127.0.0.1:8000) in your browser.

## 📖 What You'll See

An educational page explaining Python as:

- A **high-level**, beginner-friendly language
- An **interpreted** scripting language
- A tool with readable syntax, strong community support, and wide applicability

All this is served using FastAPI as an HTML page.

## 📌 Coming Soon (Ideas)

- More Python learning pages
- REST endpoints for interactive Python quizzes
- Backend + frontend separation
- Deployment instructions

## 🛠️ Dependencies

- xxx
- xxx
