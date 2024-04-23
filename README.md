# Three-Tier Application with Docker

This repository contains a three-tier application built using Docker, utilizing a multi-container setup. The application consists of three layers: presentation layer, application layer, and data layer.

## Architecture Overview

![Three-Tier Architecture](architecture_diagram.png)

- **Presentation Layer**: Responsible for presenting information to the user. Built with HTML, CSS, and JavaScript.
- **Application Layer**: Contains the business logic and functionality of the application. Built with JAVA.
- **Data Layer**: Stores and manages the data used by the application. Utilizes MYSQL.

## Getting Started

Follow these steps to run the three-tier application locally:

### Prerequisites

- Docker installed on your machine

### Steps

1. Clone this repository to your local machine:

    ```bash
    git clone <repository_url>
    ```

2. Navigate to the project directory:

    ```bash
    cd <project_directory>
    ```

3. Build the Docker images:

    ```bash
    docker-compose build
    ```

4. Start the Docker containers:

    ```bash
    docker-compose up -d
    ```

5. Access the application in your web browser:

    ```
    http://localhost:3000
    ```

## Author

- [Your Name](https://github.com/your_github_username)

## Acknowledgements

- This project is inspired by [Original Author's Name](https://github.com/original_author) and their work on [Original Project Name](https://github.com/original_project).

## Prerequisites
- JDK 1.8 or later
- Maven 3 or later
- MySQL 5.6 or later

## Technologies 
- Spring MVC
- Spring Security
- Spring Data JPA
- Maven
- JSP
- MySQL

## Database Setup
### Installation Steps for MySQL on Ubuntu 14.04
```bash
sudo apt-get update
sudo apt-get install mysql-server
```
### Importing Database Dump
1. Locate the `accountsdb.sql` file in the `/src/main/resources` directory.
2. This file contains a MySQL dump of the database schema and data.
3. Run the following command to import the dump into the MySQL database:
```bash
mysql -u <user_name> -p accounts < accountsdb.sql
```
Replace `<user_name>` with your MySQL username. You will be prompted to enter your MySQL password after running this command.
