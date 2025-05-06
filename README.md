# E-Commerce-Practical-Day06
Employee Management System

Overview:
This project is an Employee Management System built using Java with Jakarta Persistence API (JPA) for database operations. It manages relationships between employees, departments, projects, and insurance information.

Project Structure

Entity Models
The system consists of four main entities:

1. Employee
   - Primary attributes: employee number, name, age, salary, gender
   - Relationships:
     - Many-to-One with Department
     - Many-to-Many with Project
     - One-to-One with Insurance

2.Department
   - Primary attributes: ID, name, establishment date
   - Relationships:
     - One-to-Many with Employee (a department has many employees)

3. Project
   - Primary attributes: ID, name, total cost
   - Relationships:
     - Many-to-Many with Employee (a project has many employees)

4. Insurance
   - Primary attributes: ID, type
   - Relationships:
     - One-to-One with Employee

Entity Relationships
- An employee belongs to one department, but a department can have multiple employees
- An employee can work on multiple projects, and a project can have multiple employees
- An employee can have one insurance policy

