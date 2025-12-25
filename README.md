# 📚 FastAPI Book API

A simple REST API built with **FastAPI** that allows you to manage a list of books.
This project is designed for learning and practicing FastAPI basics such as
routing, request bodies, and CRUD operations.

---

## 🚀 Features

- Get all books
- Get a book by ID
- Add a new book
- Delete a book by ID
- Input validation using **Pydantic**
- Automatic API documentation (Swagger & ReDoc)

---

## 🛠️ Tech Stack

- Python 3.10+
- FastAPI
- Uvicorn
- Pydantic

---

## 📂 Project Structure

```

.
├── main.py
└── README.md

````

---

## ▶️ How to Run the Project

### 1. Create a virtual environment (optional)
```bash
python -m venv venv
source venv/bin/activate   # macOS / Linux
venv\Scripts\activate      # Windows
````

### 2. Install dependencies

```bash
pip install fastapi uvicorn
```

### 3. Start the server

```bash
uvicorn main:app --reload
```

The API will run at:

```
http://127.0.0.1:8000
```

---

## 📖 API Documentation

FastAPI automatically generates interactive documentation:

* **Swagger UI**
  [http://127.0.0.1:8000/docs](http://127.0.0.1:8000/docs)

* **ReDoc**
  [http://127.0.0.1:8000/redoc](http://127.0.0.1:8000/redoc)

---

## 🔗 API Endpoints

### Get all books

```
GET /books
```

Optional query parameter:

```
/books?limit=2
```

---

### Get a book by ID

```
GET /books/{book_id}
```

Example:

```
GET /books/1
```

---

### Add a new book

```
POST /books
```

Request body:

```json
{
  "title": "New Book",
  "author": "Author Name",
  "pages": 200
}
```

---

### Delete a book by ID

```
DELETE /books/{book_id}
```

Example:

```
DELETE /books/3
```

---

## ⚠️ Notes

* Data is stored **in memory** (list).
* All data resets when the server restarts.
* This project is for **learning purposes only**.

---

## 🌱 Future Improvements

* Add update endpoints (PUT / PATCH)
* Connect to a database (SQLite / MySQL / PostgreSQL)
* Add authentication
* Improve error handling
* Add unit tests

---

## 👤 Author

Created by **Hitomi Goto**
Learning FastAPI & backend development 🚀