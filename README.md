# Pastebin Clone API

A backend service that allows users to **store and share text or code snippets using unique links**.

Users can create a paste and receive a shareable link that allows others to view the stored content.

---

## 🚀 Features

- Create and store text/code snippets
- Generate unique links for each paste
- Retrieve stored pastes using the link
- Delete pastes
- REST API based architecture

---

## 🛠 Tech Stack

- Java
- Spring Boot
- Spring Data JPA
- MySQL / H2 Database
- Maven
- REST APIs

---

## 📂 Project Structure

```
src
 ├── controller
 │      PasteController.java
 ├── service
 │      PasteService.java
 ├── repository
 │      PasteRepository.java
 ├── model
 │      Paste.java
 └── PastebinApplication.java
```

---

## 📌 API Endpoints

### Create Paste

POST /paste

Example Request

```
{
  "content": "Hello World"
}
```

Example Response

```
{
  "pasteId": "x9k32"
}
```

---

### Retrieve Paste

GET /paste/{id}

Example

```
GET /paste/x9k32
```

Returns stored content.

---

### Delete Paste

DELETE /paste/{id}

Deletes the paste from the database.

---

## 🗄 Database Schema

```
PASTE_TABLE
-----------
id
content
created_at
```

---

## ▶️ How to Run the Project

Clone the repository

```
git clone https://github.com/yourusername/pastebin-clone-api.git
```

Navigate to project directory

```
cd pastebin-clone-api
```

Run the application

```
mvn spring-boot:run
```

Open in browser

```
http://localhost:8080
```

---

## 💡 Learning Outcomes

- Building REST APIs using Spring Boot
- Implementing CRUD operations
- Designing backend services
- Generating unique identifiers
- Managing database persistence

---

## 📈 Future Improvements

- Paste expiration feature
- Syntax highlighting for code
- User authentication
- Public/private pastes
- View analytics

---

## 👨‍💻 Author

Pranav Ganorkar
