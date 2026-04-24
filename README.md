# Online Job Portal

A simple and lightweight Online Job Portal application built using Java and Spring Boot. This system allows job seekers to search and apply for jobs, while employers can post and manage job listings efficiently.

---

## Overview

The Online Job Portal streamlines the hiring process by connecting employers and job seekers on a single platform. Employers can create job postings with detailed descriptions, and candidates can explore opportunities based on their skills and preferences. The system also supports communication and application tracking.

---

## Technologies Used

* Java 8
* Spring Boot
* Spring Security with JWT Authentication
* PostgreSQL
* Hibernate (JPA)
* Maven
* Swagger (API Documentation)
* Postman (API Testing)

---

## Software Used

* IntelliJ IDEA (Backend Development)
* PostgreSQL (Database)
* Postman (API Testing)

---

## Features

### Administrator Module

* Login to the system
* Register new administrators
* Manage job categories
* View all jobs and applicants
* Manage employers and employees

### Employer Module

* Register and login
* Post job listings
* View applicants for jobs
* Update application status

### Employee Module

* Register and login
* Search and view jobs
* Apply for jobs
* Update profile details
* Track applied jobs and status
* Cancel job applications

---

## Project Structure

```
src/
 └── main/
     ├── java/
     └── resources/
pom.xml


### Authentication

* POST `/api/auth/login` – Login and get JWT token
* POST `/api/auth/signin` – Register new user

### Employer APIs

* POST `/api/employers` – Create employer
* POST `/api/employers/{id}/jobs` – Create job
* GET `/api/employers` – Get all employers
* GET `/api/employers/{id}/jobs` – Get employer jobs
* DELETE `/api/employers/{id}/jobs/{jobId}` – Delete job

### Employee APIs

* POST `/api/employees` – Create employee
* GET `/api/employees` – Get all employees
* GET `/api/employees/{id}` – Get employee by ID
* POST `/api/employees/{id}/jobs/{jobId}/apply` – Apply for job

### Job APIs

* GET `/api/jobs` – Get all jobs
* GET `/api/jobs/{id}` – Get job by ID
* GET `/api/jobs/search` – Search jobs

---

## Database Schema

(Add your DB schema image here if needed)

---

## Setup Instructions

1. Clone the repository:

```
git clone https://github.com/vanitha00/Online_Job_Application_System.git
```

2. Open the project in IntelliJ IDEA or any IDE.

3. Configure database:

* Go to `src/main/resources/application.properties`
* Update:

  * Database URL
  * Username
  * Password

4. Run the application:

* Start Spring Boot application
* Server runs at:

```
http://localhost:8080
```

---

## Author

Kotla Vanitha

---

