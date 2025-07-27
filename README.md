### ✅ `money_manager` – Backend

**Repo:** [https://github.com/Sairammargam/money_manager](https://github.com/Sairammargam/money_manager)

```markdown
# 🧾 Money Manager Backend

A Spring Boot backend for managing personal financial transactions. It provides REST APIs for tracking expenses and incomes, user authentication, and category management.

## 🚀 Features

- ✅ Add, update, delete transactions
- 📊 Get summaries by category or date
- 🔐 User registration and login (JWT-based if implemented)
- 🔄 CORS-enabled for frontend integration
- 🧩 Category-wise spending breakdown

## 🛠️ Tech Stack

- **Spring Boot**
- **Spring Data JPA**
- **PostgreSQL / MySQL** (configurable DB)
- **Spring Security** (if enabled)
- **Swagger UI** (for API docs)

## 🗂️ Project Structure
  src/
├── controller/
├── service/
├── repository/
├── model/
├── dto/
└── MoneyManagerApplication.java
```

## 🔧 Setup Instructions

1. **Clone the repository**

```bash
git clone https://github.com/Sairammargam/money_manager.git
cd money_manager
```

2. Configure Database
   - Edit src/main/resources/application.properties:
      - spring.datasource.url=jdbc:postgresql://localhost:5432/your_db
      - spring.datasource.username=your_username
      - spring.datasource.password=your_password
      - spring.jpa.hibernate.ddl-auto=update
        
3. Run the application
   
  -  ./mvnw spring-boot:run
    
## 📬 API Endpoints Overview
| Endpoint            | Method          | Description           |
| ------------------- | --------------- | --------------------- |
| `/api/transactions` | GET/POST/DELETE | CRUD for transactions |
| `/api/categories`   | GET             | List categories       |
| `/api/users`        | POST            | User registration     |
| `/api/auth/login`   | POST            | Login                 |


