# Todo App

A Todo application built with Node.js featuring user authentication and a task management system. Users can create, read, update, and delete todos. Access tokens are used for authentication and expire after 30 minutes.

## Features

- User authentication with access tokens
- Create, read, update, and delete todos
- Token-based authentication with expiration (30 minutes)
- Secure API endpoints for managing todos

## Technologies Used

- Node.js
- Express
- MongoDB (or other database if applicable)

## Getting Started

To get a local copy up and running follow these simple steps.

### Prerequisites

- [Node.js](https://nodejs.org/) installed
- [npm](https://www.npmjs.com/) installed
- [MongoDB](https://www.mongodb.com/) (if applicable)

### Installation

1. Clone the repository:

    ```bash
    git clone https://github.com/yourusername/todo-app.git
    ```

2. Navigate to the project directory:

    ```bash
    cd todo-app
    ```

3. Install dependencies:

    ```bash
    npm install
    ```

4. Create a `.env` file in the root directory and add your environment variables, including database connection string and JWT secret.

5. Run the application:

    ```bash
    npm start
    ```

6. Open your browser and navigate to `http://localhost:3000` to view the application.

## Authentication

- **Login**: Generate an access token by providing valid credentials.
- **Token Expiration**: Access tokens expire after 30 minutes.
- **Authorization**: Use the access token in the `Authorization` header to access protected routes.

## API Endpoints

### Todos

- **Create a Task**
  
  `POST /api/todos`
  
  Request body:
  ```json
  {
    "title": "Task title",
    "description": "Task description"
  }
