# Coursera Clone

This project is a clone of the Coursera platform, built using React for the frontend and Express.js for the backend. It allows users to browse and purchase courses, and administrators to manage courses.

## Table of Contents

- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [API Endpoints](#api-endpoints)
- [Contributing](#contributing)
- [License](#license)

## Features

- User authentication (signup, login)
- Admin authentication (signup, login)
- Course management (add, update, delete courses)
- Purchase courses

## Installation

1. Clone the repository:
    ```sh
    git clone https://github.com/yourusername/coursera-clone.git
    cd coursera-clone
    ```

2. Install dependencies for the backend:
    ```sh
    cd backend
    npm install
    ```

3. Install dependencies for the frontend:
    ```sh
    cd ../frontend
    npm install
    ```

4. Set up environment variables:
    - Create a `.env` file in the `backend` directory and add the following:
        ```
        MONGODB_URI=your_mongodb_connection_string
        JWT_SECRET=your_jwt_secret
        ```

## Usage

1. Start the backend server:
    ```sh
    cd backend
    npm start
    ```

2. Start the frontend development server:
    ```sh
    cd ../frontend
    npm run dev
    ```

3. Open your browser and navigate to `http://localhost:3000` to view the application.

## API Endpoints

### Admin

- `POST /admin/signup`: Sign up as an admin
- `POST /admin/signin`: Sign in as an admin
- `GET /admin/me`: Get admin details
- `POST /admin/addcourse`: Add a new course
- `PUT /admin/course/:courseId`: Update a course
- `DELETE /admin/delete-course/:courseId`: Delete a course
- `GET /admin/course/:courseId`: Get course details
- `GET /admin/course`: Get all courses

### User

- `POST /user/signup`: Sign up as a user
- `POST /user/courses/:courseId`: Purchase a course

## Contributing

Contributions are welcome! Please open an issue or submit a pull request.

## License

This project is licensed under the MIT License.
