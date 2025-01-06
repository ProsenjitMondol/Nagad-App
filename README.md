# Nagad App Project

## Overview

This project is a Java-based implementation of the Nagad App, a digital payment platform that provides seamless financial transactions such as money transfers, bill payments, and mobile recharges. The application is designed to be scalable, secure, and user-friendly.

## Features

- **User Authentication:** Secure login and registration.
- **Money Transfer:** Send and receive money instantly.
- **Bill Payments:** Pay utility bills with ease.
- **Mobile Recharge:** Recharge mobile balances for all major telecom operators.
- **Transaction History:** View and download transaction records.
- **Multi-language Support:** Provides support for multiple languages.

## Technologies Used

- **Programming Language:** Java
- **Frameworks:**
  - Spring Boot (Backend)
  - Hibernate (ORM for database interaction)
- **Database:** MySQL
- **Build Tool:** Maven
- **Version Control:** Git
- **API Documentation:** Swagger
- **Testing:** JUnit, Mockito

## Prerequisites

To run this project, ensure you have the following installed:

- **Java Development Kit (JDK):** Version 11 or later
- **Maven:** For building the project
- **MySQL:** For database
- **Git:** For version control

## Installation

1. **Clone the Repository:**
   ```bash
   git clone https://github.com/your-username/nagad-app.git
   ```
2. **Navigate to the Project Directory:**
   ```bash
   cd nagad-app
   ```
3. **Configure Database:**
   - Create a database named `nagad_app` in MySQL.
   - Update the `application.properties` file with your MySQL credentials:
     ```properties
     spring.datasource.url=jdbc:mysql://localhost:3306/nagad_app
     spring.datasource.username=your_username
     spring.datasource.password=your_password
     ```
4. **Build the Project:**
   ```bash
   mvn clean install
   ```
5. **Run the Application:**
   ```bash
   mvn spring-boot:run
   ```

## API Endpoints

| Endpoint             | Method | Description              |
| -------------------- | ------ | ------------------------ |
| `/api/auth/login`    | POST   | User login               |
| `/api/auth/register` | POST   | User registration        |
| `/api/transfer`      | POST   | Money transfer           |
| `/api/bill-payment`  | POST   | Pay utility bills        |
| `/api/recharge`      | POST   | Mobile recharge          |
| `/api/transactions`  | GET    | View transaction history |

For detailed API documentation, access Swagger at `http://localhost:8080/swagger-ui.html` after running the application.

## Folder Structure

```
|-- src
    |-- main
        |-- java
            |-- com.nagad
                |-- controller  # REST controllers
                |-- service     # Business logic
                |-- repository  # Data access layer
                |-- model       # Entity classes
        |-- resources
            |-- application.properties  # Configuration file
    |-- test
        |-- java
            |-- com.nagad       # Unit and integration tests
```

## Contributing

We welcome contributions! To contribute:

1. Fork the repository.
2. Create a new branch for your feature or bug fix:
   ```bash
   git checkout -b feature-name
   ```
3. Commit your changes and push to your branch.
   ```bash
   git push origin feature-name
   ```
4. Open a pull request.

## License

This project is licensed under the [MIT License](LICENSE).

## Contact

For any queries or support, please contact:

- **Email:** [support@nagadapp.com](mailto\:support@nagadapp.com)
- **GitHub Issues:** [GitHub Issues](https://github.com/your-username/nagad-app/issues)

---

Thank you for using the Nagad App! We hope it simplifies your digital financial transactions.
