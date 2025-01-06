## Overview
Project Service is a backend service designed for managing projects and related metadata. This service provides a robust API for creating, updating, retrieving, and deleting project records, as well as handling associated functionalities like file uploads and status management.

## Features
- **Project Management:** Create, update, delete, and retrieve project details.
- **File Upload:** Supports uploading cover images for projects.
- **Flexible Integration:** Exposes a REST API for seamless integration with other services.
- **Error Handling:** Includes custom exceptions for clear and structured error responses.
- **Swagger Documentation:** Comprehensive API documentation for developers.

## Getting Started

### Prerequisites
- Java 17
- Docker (optional, for containerized deployment)
- Gradle

### Steps
1. Clone the repository:
  
   git clone https://github.com/IvanMatiko/project_service.git
   cd project_service/project_service

2.Build the project:
  
  ./gradlew build

3.Run the application:

  ./gradlew bootRun

4.(Optional) Build and run with Docker:

  docker build -t project-service .
  docker run -p 8080:8080 project-service

# API Endpoints
GET /projects: Retrieve a list of projects.
POST /projects: Create a new project.
PUT /projects/{id}: Update an existing project.
DELETE /projects/{id}: Delete a project by ID.
For detailed API specifications, refer to the Swagger documentation.

# Technologies Used
Java: Core programming language.
Spring Boot: Framework for building the backend service.
PostgreSQL: used like relational DB
Redis: cache and like broker of messages
Gradle: Build automation tool.
Liquibase: migration of DB
Swagger: API documentation.
Docker: For containerized deployments.
