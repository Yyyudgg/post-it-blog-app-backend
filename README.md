# Post-It Blog App Backend 🚀

![Post-It Blog App](https://img.shields.io/badge/Post--It%20Blog%20App%20Backend-Node.js%20%7C%20Express%20%7C%20MongoDB-blue)

Welcome to the **Post-It Blog App Backend** repository! This project serves as the backend for a MERN stack blog application. It includes user authentication, password security, and a complete CRUD API for managing blog posts. Below, you'll find detailed information about the project, including installation instructions, usage, and contribution guidelines.

## Table of Contents

1. [Project Overview](#project-overview)
2. [Features](#features)
3. [Technologies Used](#technologies-used)
4. [Installation](#installation)
5. [Usage](#usage)
6. [API Endpoints](#api-endpoints)
7. [Authentication](#authentication)
8. [Contributing](#contributing)
9. [License](#license)
10. [Releases](#releases)
11. [Contact](#contact)

## Project Overview

The **Post-It Blog App Backend** is designed to provide a seamless experience for users looking to create, read, update, and delete blog posts. It leverages the power of Node.js and Express to build a RESTful API, while MongoDB serves as the database for storing user and post data. The application also implements JWT-based authentication for secure user sessions.

## Features

- **User Authentication**: Secure user login and registration using JWT.
- **Password Security**: Passwords are hashed using bcrypt to enhance security.
- **CRUD Operations**: Create, read, update, and delete blog posts with ease.
- **RESTful API**: Well-structured API endpoints for easy integration.
- **Scalability**: Built with scalability in mind, suitable for future enhancements.

## Technologies Used

- **Node.js**: JavaScript runtime for building server-side applications.
- **Express**: Web framework for Node.js, used for building APIs.
- **MongoDB**: NoSQL database for storing data.
- **Mongoose**: ODM for MongoDB and Node.js.
- **JWT**: JSON Web Tokens for secure authentication.
- **bcrypt**: Library for hashing passwords.

## Installation

To get started with the Post-It Blog App Backend, follow these steps:

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/Yyyudgg/post-it-blog-app-backend.git
   cd post-it-blog-app-backend
   ```

2. **Install Dependencies**:
   Run the following command to install the necessary packages:
   ```bash
   npm install
   ```

3. **Environment Variables**:
   Create a `.env` file in the root directory and add the following variables:
   ```
   PORT=5000
   MONGODB_URI=your_mongodb_connection_string
   JWT_SECRET=your_jwt_secret
   ```

4. **Start the Server**:
   Use the following command to start the server:
   ```bash
   npm start
   ```

Your backend server should now be running on `http://localhost:5000`.

## Usage

Once the server is running, you can use tools like Postman or Insomnia to interact with the API. The API endpoints allow you to manage blog posts and user authentication.

## API Endpoints

Here are the main API endpoints available in the Post-It Blog App Backend:

### User Authentication

- **Register a new user**:
  - `POST /api/auth/register`
  - Body: `{ "username": "your_username", "password": "your_password" }`

- **Login a user**:
  - `POST /api/auth/login`
  - Body: `{ "username": "your_username", "password": "your_password" }`

### Blog Posts

- **Create a new post**:
  - `POST /api/posts`
  - Headers: `Authorization: Bearer your_jwt_token`
  - Body: `{ "title": "Post Title", "content": "Post Content" }`

- **Get all posts**:
  - `GET /api/posts`

- **Get a single post**:
  - `GET /api/posts/:id`

- **Update a post**:
  - `PUT /api/posts/:id`
  - Headers: `Authorization: Bearer your_jwt_token`
  - Body: `{ "title": "Updated Title", "content": "Updated Content" }`

- **Delete a post**:
  - `DELETE /api/posts/:id`
  - Headers: `Authorization: Bearer your_jwt_token`

## Authentication

The application uses JWT for user authentication. After a successful login, the server generates a token that the client must include in the `Authorization` header for protected routes. This token allows the server to verify the user's identity.

## Contributing

Contributions are welcome! If you would like to contribute to this project, please follow these steps:

1. Fork the repository.
2. Create a new branch: `git checkout -b feature/YourFeature`.
3. Make your changes and commit them: `git commit -m 'Add some feature'`.
4. Push to the branch: `git push origin feature/YourFeature`.
5. Open a Pull Request.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Releases

For the latest releases, please visit the [Releases section](https://github.com/Yyyudgg/post-it-blog-app-backend/releases). You can download the latest version and execute it as needed.

## Contact

For any inquiries or feedback, feel free to reach out:

- **GitHub**: [Yyyudgg](https://github.com/Yyyudgg)
- **Email**: your-email@example.com

Thank you for checking out the Post-It Blog App Backend! We hope you find it useful.