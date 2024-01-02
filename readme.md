# Docker Compose DIO Project

This project is a part of a course on Docker and Docker Compose. The goal of the project is to create a multi-container application using Docker Compose.

## Project Structure

The project consists of three services:

1. **Angular App**: This service is built from the `./angular-app` directory and exposes port 4200. The application files are mounted from the host to the container at `/usr/local/fudgelate-webpage/angular-app`.

2. **Java App**: This service is built from the `./java-app` directory and exposes port 8080. It depends on the `db` service. The application files are mounted from the host to the container at `/usr/local/fudgelate-webpage/java-app`.

3. **Database**: This service uses the latest PostgreSQL image. It sets up a database with the username `postgres`, password `postgres`, and database name `mydatabase`. It exposes port 5432 and mounts the data directory from the host to the container at `/usr/local/fudgelate-webpage/db-data`.

## Running the Application

To run the application, navigate to the project directory and execute the following command:

bash docker-compose up

This will start all the services defined in the `docker-compose.yml` file.

## Course Objectives

The course objectives were to create a server with Apache (httpd), specify the location of the application files in the YML file, and run a complete web application. The students were also encouraged to push the YML file and the application to a GitHub repository.

However, I took the challenge a bit further and implemented a more complex setup with Angular, Java, and PostgreSQL services. I believe this setup provides a more realistic representation of a full-stack web application.

## Contributing

Feel free to fork the repository and make improvements. Any contributions you make are greatly appreciated.
You can copy this content and paste it into your README file.