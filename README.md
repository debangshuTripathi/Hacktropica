# Ecyclehub

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

## Project Description

EcycleHub is a web application developed in Java that bridges the gap between individuals who wish to donate reusable products and organizations that seek to repurpose them. In today’s fast-paced world, reusable items such as clothes, electronics, furniture, and books are discarded daily, contributing to environmental waste. At the same time, many NGOs, businesses, and social organizations are in constant need of such items.

EcycleHub provides a sustainable digital platform where:

- *Public users* can donate recyclable products with proper location, name, and contact information.
- *Organizers* can access the donated items, review the submissions, and make arrangements to reuse or distribute them.

By encouraging reuse, EcycleHub supports a *circular economy, reduces landfill waste, and promotes community-driven environmental change. This platform aims to ensure that **nothing goes to waste, and every product gets a **second chance*!

👉 GitHub Repository: [https://github.com/debangshuTripathi/Hacktropica](https://github.com/debangshuTripathi/Hacktropica)

---

## Features and Functionality

- *Item Donation by Public:*  
  Users can donate items by submitting details such as item name, category, location (state, district, city, pin code), and contact number.

- *Organizer Access:*  
  Organizers can view all submitted items, review them, and make decisions for reuse or redistribution.

- *Location-Based Listing:*  
  Items are listed along with their location details, helping organizers identify region-specific donations.

- *Sustainability Focus:*  
  Encourages reducing pollution and supporting environmental welfare through reuse of recyclable materials.

- *Dynamic Web Pages (JSP):*  
  The platform provides simple and intuitive JSP pages for item addition, viewing items, and displaying success messages.

---

## Technology Stack

- *Backend:*
  - Java 17
  - Spring Boot (Spring Web, Spring Data JPA)
  - Hibernate
  - Lombok

- *Frontend:*
  - HTML, CSS
  - JSP (Java Server Pages)

- *Database:*
  - PostgreSQL

- *Build & Tools:*
  - Maven (build tool)
  - IntelliJ IDEA (IDE)
  - GitHub (version control & deployment)

---

## Prerequisites

Before running the application, make sure you have:

- *Java Development Kit (JDK):* Version 17
- *Maven:* Installed and configured
- *IntelliJ IDEA:* Preferred IDE
- *PostgreSQL Database:* Running locally and configured

---

## Installation Instructions

### 1. Clone the Repository:

bash
git clone https://github.com/debangshuTripathi/Hacktropica.git
cd Hacktropica


### 2. Configure the Database:

Update your src/main/resources/application.properties with the following:

properties
spring.application.name=newwwwww
spring.mvc.view.prefix=/views/
spring.mvc.view.suffix=.jsp

# PostgreSQL Database Configuration
spring.datasource.url=jdbc:postgresql://localhost:5432/debangshu
spring.datasource.username=postgres
spring.datasource.password=132004
spring.datasource.driver-class-name=org.postgresql.Driver

# Hibernate Properties
spring.jpa.database-platform=org.hibernate.dialect.PostgreSQLDialect
spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=true


Ensure PostgreSQL is running and the database debangshu exists.

### 3. Build the Application:

bash
mvn clean install


### 4. Run the Application:

bash
mvn spring-boot:run


Or using the JAR:

bash
java -jar newwwwww/target/newwwwww-0.0.1-SNAPSHOT.jar


---

## Usage Guide

### 1. Access the Web App:

Open a browser and go to:  
[http://localhost:8080/](http://localhost:8080/)

### 2. Available Endpoints:

- *Home Page:*  
  /home – Starting point of the application

- *Donate Item:*  
  /addItem – Form page to donate items (item name, location, product type, contact number)

- *Success Page:*  
  /success – Confirmation page after successful submission

- *All Items List:*  
  /allItem – Displays all donated items for organizers

---

## API Documentation

This application is a *web-based JSP application* and does not expose a REST API. However, it includes the following internal endpoints:

- GET /home → Loads the home page
- GET /addItem → Loads the donation form
- POST /success → Submits the donation and stores it
- GET /allItem → Displays all donated items from the database

---

## Contributing Guidelines

Contributions are welcome!

1. Fork the repository
2. Create a new branch (feature-xyz)
3. Add your features or bug fixes
4. Commit with proper messages
5. Submit a pull request with a detailed description

---

## License Information

This project is licensed under the MIT License – see the [LICENSE](LICENSE) file for details.

---

## Contact / Support

For queries or support, please raise an issue in the GitHub repository:  
👉 [https://github.com/debangshuTripathi/Hacktropica/issues](https://github.com/debangshuTripathi/Hacktropica/issues)

---

Let me know if you'd like this as a downloadable .md file or want help uploading it to your repository!
