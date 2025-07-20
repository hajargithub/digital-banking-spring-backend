
# 💳 Digital Banking Spring Backend

A secure and scalable digital banking backend system built using **Spring Boot**, **Spring Security**, **JWT**, **JPA (Hibernate)**, and **MySQL**.

---

## 🚀 Features

- 🧑‍💼 Customer and Account Management
- 💸 Account Operations (Credit, Debit)
- 🔒 JWT-based Authentication
- 🛡️ Role-based Authorization
- 📈 REST APIs with Swagger UI
- 📄 Audit and Logging (optional)
- 🧪 Unit & Integration Testing Support

---

## 📂 Project Structure

```
digital-banking-spring-backend/
├── src/
│   ├── main/
│   │   ├── java/
│   │   │   └── ma.enset.ebankingbackend/
│   │   │       ├── entities/
│   │   │       ├── repositories/
│   │   │       ├── services/
│   │   │       ├── security/
│   │   │       ├── web/
│   │   │       └── dtos/
│   │   └── resources/
│   │       └── application.properties
├── pom.xml
└── README.md
```

---

## ⚙️ Technologies Used

| Tech                | Description                            |
|---------------------|----------------------------------------|
| Spring Boot         | Backend framework                      |
| Spring Data JPA     | ORM with Hibernate                     |
| Spring Security     | Secure endpoints with JWT              |
| Lombok              | Boilerplate code reduction             |
| MySQL               | Relational database                    |
| Swagger / OpenAPI   | API Documentation                      |
| Maven               | Build and dependency management        |

---

## 🛠️ Getting Started

### 1. Clone the repo
```bash
git clone https://github.com/hajargithub/digital-banking-spring-backend.git
cd digital-banking-spring-backend
```

### 2. Configure the database

Ensure MySQL is running and update credentials in `src/main/resources/application.properties`:

```properties
spring.datasource.url=jdbc:mysql://localhost:3306/digital_banking_db?createDatabaseIfNotExist=true&useSSL=false
spring.datasource.username=root
spring.datasource.password=
spring.jpa.hibernate.ddl-auto=update
spring.jpa.properties.hibernate.dialect=org.hibernate.dialect.MySQL8Dialect
```

---

### 3. Run the application

You can start the application using IntelliJ or from the terminal:

```bash
./mvnw spring-boot:run
```

The app will run at: `http://localhost:8085`

---

## 🔐 Authentication

This project uses **JWT (JSON Web Tokens)** for securing endpoints.

You can set the JWT secret in your `application.properties`:

```properties
jwt.secret=yourStrongSecretKeyHere
```

---

## 📬 API Documentation

Once the app is running, access Swagger UI:

👉 [http://localhost:8085/swagger-ui.html](http://localhost:8085/swagger-ui.html)

---

## 🧪 Running Tests

```bash
./mvnw test
```

---



