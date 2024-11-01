# 832202120_concacts_Backend

```markdown
# Spring Boot Employee Management System

## Overview

This repository contains a Spring Boot application designed to manage employee data. The application provides a RESTful API to perform CRUD (Create, Read, Update, Delete) operations on employee records.

## Features

- Add new employees
- Update existing employee information
- Delete employees by ID or in batch
- Retrieve all employees or by specific ID
- Search employees with pagination

## Prerequisites

- Java JDK 11 or higher
- MySQL Server
- Maven or Gradle for building the project
- IDE (Eclipse, IntelliJ IDEA, etc.) or Text Editor

## Setup

1. Clone the repository:
   ```
   git clone [repository-url]
   ```
   Replace `[repository-url]` with the URL of your repository.

2. Import the project into your IDE.

3. Configure the database connection in `application.yml` or `application.properties` file:
   ```yaml
   spring:
     datasource:
       driver-class-name: com.mysql.cj.jdbc.Driver
       username: root
       password: 123456
       url: jdbc:mysql://localhost:3306/xm?useUnicode=true&characterEncoding=utf-8&allowMultiQueries=true&useSSL=false&serverTimezone=GMT%2b8&allowPublicKeyRetrieval=true
   ```

4. Run the application:
   ```
   mvn spring-boot:run
   ```
   or using your IDE's run configuration.

5. Access the API endpoints to manage employee data.

## API Documentation

- **Add Employee**
  `POST /employee/add`
  - Request Body: `Employee` object

- **Update Employee**
  `PUT /employee/update`
  - Request Body: `Employee` object

- **Delete Employee by ID**
  `DELETE /employee/deleteById/{id}`

- **Delete Batch of Employees**
  `DELETE /employee/deleteBatch`
  - Request Body: `List<Integer>` of IDs

- **Select All Employees**
  `GET /employee/selectAll`
  - Request Parameter: `Employee` object (optional)

- **Select Employee by ID**
  `GET /employee/selectById/{id}`

- **Select Employees with Pagination**
  `GET /employee/selectPage`
  - Request Parameter: `Employee` object (optional)
  - Query Parameters: `pageNum` (default: 1), `pageSize` (default: 10)

## Contributing

Contributions are welcome! Please follow the standard GitHub workflow:
1. Fork the repository.
2. Create a new branch for your changes.
3. Make your changes and test thoroughly.
4. Submit a pull request with a detailed description of your changes.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
```

