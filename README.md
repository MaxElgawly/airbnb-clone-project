\# AirBnB Clone Project



\## Overview

This project is a simplified clone of the AirBnB platform. It is part of the ALX Software Engineering curriculum and aims to teach full-stack development using foundational tools and technologies.



\## Goals

\- Understand the concept of Object-Oriented Programming (OOP)

\- Learn how to manage projects with Git and GitHub

\- Build a full-stack web application with data persistence



\## Tech Stack

\- Python (backend logic)

\- MySQL or other database (data storage)

\- Flask or another web framework

\- HTML/CSS (frontend)

\- Git \& GitHub (version control)







## Team Roles

### 1. Backend Developer
Responsible for building the core business logic, APIs, and server-side functionality. Ensures that data flows correctly between the database and the frontend.

### 2. Frontend Developer
Focuses on designing and developing the user interface. Works with HTML, CSS, and JavaScript to create a responsive and interactive user experience.

### 3. Database Administrator (DBA)
Manages the database schema, ensures data integrity, sets up queries, and optimizes database performance for the application.

### 4. DevOps Engineer
Handles version control, deployment pipelines, and automates infrastructure using CI/CD tools. Ensures smooth integration and continuous delivery.

### 5. Project Manager
Coordinates the team’s efforts, sets deadlines, assigns responsibilities, and ensures the project stays on track.

### 6. QA Engineer (Tester)
Tests the application thoroughly to catch bugs and ensure quality standards are met before any release.




## Technology Stack

- **Python**: The primary programming language used to build backend logic and system functionality.

- **Django**: A high-level Python web framework used to develop robust and scalable web applications, including RESTful APIs.

- **PostgreSQL**: A powerful open-source relational database system used to store and manage data persistently.

- **HTML/CSS**: Used to build and style the user interface of the web application.

- **JavaScript**: Adds interactivity and dynamic content handling in the frontend.

- **GraphQL**: A query language for APIs that allows clients to request exactly the data they need, improving performance and flexibility.

- **Git**: Version control tool used to manage source code changes across the team.

- **GitHub**: Hosts the code repository and facilitates collaboration via pull requests and issues.

- **Docker** (optional, if mentioned): Used to containerize the application for easier development and deployment across environments.

- **CI/CD Tools** (e.g., GitHub Actions): Automate testing, building, and deploying of the application.



## Database Design

### 1. Users
- **id**: unique identifier
- **name**: full name of the user
- **email**: user’s email address
- **password_hash**: securely stored password
- **role**: host or guest

### 2. Properties
- **id**: unique property ID
- **owner_id**: reference to the user (host)
- **title**: property title
- **location**: address or city
- **price_per_night**: rental cost

### 3. Bookings
- **id**: unique booking ID
- **user_id**: the guest who made the booking
- **property_id**: the property being booked
- **start_date**: check-in date
- **end_date**: check-out date

### 4. Reviews
- **id**: unique review ID
- **booking_id**: related booking
- **user_id**: who left the review
- **rating**: numerical score (e.g., 1 to 5)
- **comment**: optional text feedback

### 5. Payments
- **id**: unique payment ID
- **booking_id**: the booking being paid for
- **amount**: total payment amount
- **payment_method**: e.g., credit card, PayPal
- **status**: success, pending, failed
