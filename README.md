# todolist - Java

A todolist application in Java 17

## Technologies

- Spring Boot
- APIDog
- Maven
- H2 (DataBase)
- Render (for deploy)
- Outras bibliotecas e pacotes

## Description

This is a simple todolist application built using Java 17 and Spring Boot. The application uses H2 as its database and is deployed on Render using Docker.

To run the application locally, you can use the following command:

```mvn spring-boot:run```

## You can use the ApiDog to test the application.

functionality:

- Create a user
- Create a task
  - The task must have a title, description, date and time
  - The task must be associated with a user
  - The start date and time must be greater than the current date and time
  - The end date and time must be greater than the start date and time
  - Every time a task is created or listed, it authenticates the username and password
  - Every time a task is created or listed, it checks if the task exist through the id
- List all tasks
