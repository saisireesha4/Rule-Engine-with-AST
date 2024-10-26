Rule Engine with Abstract Syntax Tree (AST) for Eligibility Evaluation
This project implements a rule engine using an Abstract Syntax Tree (AST) for parsing and evaluating user eligibility based on dynamically defined rules. The application uses Flask for the web interface, MySQL for database storage, and SQLAlchemy as the ORM layer. The application is containerized using Docker to facilitate easy setup and deployment.

Key Features
Dynamic Rule Parsing and Evaluation: Allows defining and updating custom eligibility rules based on user attributes (age, income, department).
AST-based Logic Parsing: Uses AST for complex condition parsing with logical operators (AND, OR).
Web Interface with Flask: A user-friendly interface for input and result display.
MySQL Database Integration: Persistent rule storage and management.
Containerized with Docker: Application and database run as Docker containers for ease of deployment.
Design Choices
Abstract Syntax Tree (AST): Used to parse and evaluate conditions dynamically based on user input, enhancing flexibility for complex rules.
Flask for Web Framework: Lightweight framework for handling web requests and rendering templates.
MySQL Database: Relational database for storing rules and user data, supporting complex querying for rule conditions.
Docker Containerization: Simplifies setup by containerizing application and database, enabling consistent development and deployment environments.
Prerequisites
Docker and Docker Compose for container setup
Optional (if running without Docker):
Python 3.x
MySQL Database
Dependencies
Flask - Web framework
Flask_SQLAlchemy - ORM for database operations
MySQL Connector - For connecting Flask with MySQL
Application Structure
app.py: Main application file for routes, database connection, and rule evaluation.
backend/ast.py: Contains AST logic for parsing and evaluating rule conditions.
templates/: HTML templates for input (index.html) and result display (result.html).
static/: Static assets (CSS for styling).