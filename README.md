# 📚 Book Management REST API

A simple REST API built with Node.js and Express for managing a list of books using in-memory storage (no database required).

## 🛠 Tools Used

- Node.js
- Express.js
- Postman (for testing)

---

## 📦 Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/yourusername/book-api.git
cd book-api

2. Install Dependencies

npm install

3. Start the Server

node index.js

Server will run at:
http://localhost:3000


---

📘 API Endpoints

GET /books

Returns all books in the system.

Example Response:

[
  {
    "id": 1,
    "title": "1984",
    "author": "abcd"
  }
]


---

POST /books

Add a new book.

Request Body:

{
  "title": "The rabbit",
  "author": "krishnan"
}

Success Response:

{
  "id": 2,
  "title": "The rabbit",
  "author": "krishnan"
}


---

PUT /books/:id

Update a book by ID.

Example URL: /books/1

Request Body (any or both fields):

{
  "title": "Animal Farm"
}

Success Response:

{
  "id": 1,
  "title": "Animal Farm",
  "author": "George Orwell"
}


---

DELETE /books/:id

Delete a book by ID.

Example URL: /books/1

Success Response:

{
  "id": 1,
  "title": "Animal Farm",
  "author": "George Orwell"
}


---
