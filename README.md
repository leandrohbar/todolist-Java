# TodoList Application in Java 17

This is a straightforward yet efficient TodoList application developed in Java 17, leveraging the power of Spring Boot framework. The application facilitates task management, allowing users to create tasks associated with a user account, set deadlines, and maintain a structured list of pending tasks. The system utilizes H2 as its database and is deployable via Docker on platforms like Render.

## Table of Contents

- [Technologies Used](#technologies-used)
- [Features](#features)
- [Getting Started](#getting-started)
- [API Usage](#api-usage)
- [Contributing](#contributing)
- [License](#license)

## Technologies Used

- **Spring Boot:** Providing a robust framework for building and deploying Java applications.
- **APIDog:** Utilized for testing the application endpoints and functionalities.
- **Maven:** Dependency management and build automation.
- **H2 (Database):** Embedded relational database for managing application data.
- **Render (for deploy):** Deployment tool to host the application using Docker.
- **Other Libraries and Packages:** Additional libraries and packages enhancing the application's capabilities.

## Features

- **User Creation:** Allows the creation of user accounts for task management.
- **Task Creation:**
  - Each task comprises a title, description, date, and time.
  - Tasks are linked with respective users.
  - Validations:
    - Start date and time must be in the future.
    - End date and time must be after the start date and time.
    - Authentication of username and password on task creation or listing.
    - Validation of task existence based on the ID for creation or listing.
- **Task Listing:** Displays a comprehensive list of all tasks available.

## Getting Started

To run the application locally, follow these steps:

1. Clone the repository:

    ```bash
    git clone https://github.com/leandrohbar/todolist-Java.git
    ```

2. Navigate to the project directory:

    ```bash
    cd todolist-Java
    ```

3. Run the application using Maven:

    ```bash
    mvn spring-boot:run
    ```

4. Access the application on `localhost` with the defined port (e.g., `http://localhost:8080`).

## API Usage

API endpoints and functionalities:

- `POST /api/users/create`: Create a new user.
- `POST /api/tasks/create`: Create a new task with specific details.
  - Task details include title, description, date, and time.
  - Task is associated with a user.
  - Validations ensure proper scheduling and user authentication.
- `GET /api/tasks/list`: List all available tasks.

Ensure to utilize APIDog or similar tools to test and interact with the API endpoints, sending appropriate requests and receiving responses.

## Contributing

Contributions to enhance the project are welcome! Feel free to fork the repository, make changes, and create pull requests. For major modifications, please open an issue first to discuss the proposed changes.

## License

This project is licensed under the [MIT License](LICENSE.md).
