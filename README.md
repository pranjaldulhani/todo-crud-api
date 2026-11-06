# Todo CRUD API (Spring Boot)

A simple REST API to create, read, update and delete Todo items, built with Spring Boot, Spring Data JPA and H2 database.

## Tech Stack
- Java 17
- Spring Boot 4.1.2
- Spring Data JPA
- H2 In-Memory Database
- Maven

## How to Run
```
.\mvnw spring-boot:run
```
The server starts at `http://localhost:8080`

## Todo Fields
| Field | Type | Description |
|-------|------|-------------|
| id | Long | Auto-generated id |
| title | String | Todo title |
| completed | boolean | Completion status |

## API Endpoints
| Method | URL | Description |
|--------|-----|-------------|
| GET | /api/todos | Get all todos |
| GET | /api/todos/{id} | Get todo by id |
| POST | /api/todos | Create a new todo |
| PUT | /api/todos/{id} | Update a todo |
| DELETE | /api/todos/{id} | Delete a todo |

## Sample Request (POST /api/todos)
```json
{
  "title": "Learn Spring Boot",
  "completed": false
}
```

## Sample Response
```json
{
  "id": 1,
  "title": "Learn Spring Boot",
  "completed": false
}
```

## Testing
All endpoints were tested using Postman.