# CRUD Application

## Overview
This project is a simple CRUD (Create, Read, Update, Delete) application for managing person details, such as name, email, and phone number. The application is built using Java, Spring Boot, Spring Data JPA, MySQL, Thymeleaf, HTML, and CSS. It demonstrates the implementation of CRUD operations with a user-friendly interface.

---

## Features
1. Add new person details (name, email, phone number).
2. View all person records.
3. Update existing person details.
4. Delete person records.

---

## Technologies Used
- **Backend:** Java, Spring Boot, Spring Data JPA
- **Frontend:** HTML, CSS, Thymeleaf
- **Database:** MySQL

---

## Prerequisites
Make sure you have the following installed on your system:

1. Java (JDK 8 or higher)
2. Maven
3. MySQL
4. IDE (e.g., IntelliJ IDEA, Eclipse, or Visual Studio Code)

---

## Getting Started

### 1. Clone the Repository
```bash
git clone https://github.com/your-username/crud-application.git
cd crud-application
```

### 2. Configure the Database
1. Create a database in MySQL:
   ```sql
   CREATE DATABASE crud_application;
   ```
2. Update the database configuration in `application.properties`:
   ```properties
   spring.datasource.url=jdbc:mysql://localhost:3306/crud_application
   spring.datasource.username=your_mysql_username
   spring.datasource.password=your_mysql_password
   spring.jpa.hibernate.ddl-auto=update
   ```

### 3. Run the Application
1. Build the project using Maven:
   ```bash
   mvn clean install
   ```
2. Start the application:
   ```bash
   mvn spring-boot:run
   ```
3. Open your browser and go to:
   ```
   http://localhost:8080
   ```

---

## Project Structure
```
crud-application/
├── src/
│   ├── main/
│   │   ├── java/
│   │   │   └── com.example.crud/
│   │   │       ├── controller/
│   │   │       ├── entity/
│   │   │       ├── repository/
│   │   │       └── service/
│   │   ├── resources/
│   │   │       ├── templates/   # Thymeleaf templates
│   │   │       ├── static/       # CSS files
│   │   │       └── application.properties
├── pom.xml
└── README.md
```

---

## API Endpoints
| Method | Endpoint         | Description             |
|--------|------------------|-------------------------|
| GET    | `/`              | View all person details |
| GET    | `/add`           | Show add person form    |
| POST   | `/add`           | Save new person         |
| GET    | `/edit/{id}`     | Show edit person form   |
| POST   | `/update/{id}`   | Update person details   |
| GET    | `/delete/{id}`   | Delete person           |

---
## How It Works
1. **Add Person:** Fill out the form with name, email, and phone number. Submit to add a new person.
2. **View Records:** The home page displays a list of all persons with their details.
3. **Update Record:** Click the edit button next to a record, make changes, and save.
4. **Delete Record:** Click the delete button next to a record to remove it from the database.

---

## Contributing
Contributions are welcome! Feel free to submit a pull request or open an issue.

---

## Contact
For any inquiries, reach out at: parthasarathythankavel@gmail.com.com

