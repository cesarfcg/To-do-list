 # 📝 To-Do List API

![Java](https://img.shields.io/badge/Java-17+-red)
![Spring Boot](https://img.shields.io/badge/Spring%20Boot-3.x-brightgreen)
![Build](https://img.shields.io/badge/build-passing-success)

A RESTful API for task management built with **Java and Spring Boot**.  
Designed to demonstrate clean architecture, best practices, and CRUD operations.

---

## 🚀 Tech Stack
- Java 17+
- Spring Boot
- Spring Data JPA
- Maven
- MySQL
- Swagger (Springdoc OpenAPI)

---

## ⚙️ Database Configuration (MySQL)

```
src/main/resources/application.properties
```

```properties
spring.datasource.url=jdbc:mysql://localhost:3306/todo_db
spring.datasource.username=root
spring.datasource.password=your_password

spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=true
spring.jpa.database-platform=org.hibernate.dialect.MySQL8Dialect
```

---

## ▶️ Running the Application

```bash
git clone https://github.com/cesarfcg/To-do-list.git
cd todo-api
./mvnw spring-boot:run
```

```
http://localhost:8080
```

---

## 📖 API Documentation

```
http://localhost:8080/swagger-ui.html
```

### 📷 Preview
![Swagger UI](./docs/swagger.png)

---

## 📌 Endpoints

| Method | Endpoint     |
|--------|-------------|
| GET    | /todos     |
| GET    | /todos/{id} |
| POST   | /todos      |
| PUT    | /todos/{id} |
| DELETE | /todos/{id} |

---

## ⚠️ Common Issues

- Swagger not loading → ensure app is running
- MySQL connection failed → verify credentials
- Port in use → change with `server.port=8081`

---

## 👤 Author

**Fernando César**  
- GitHub: https://github.com/cesarfcg  
- LinkedIn: https://linkedin.com/

---

