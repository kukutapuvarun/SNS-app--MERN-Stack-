![SNS App](https://github.com/user-attachments/assets/54990cf9-f861-4411-b480-185416fd2e3c)

# SNS App

A Social Networking Service (SNS) application built using the MERN stack (MongoDB, Express.js, React, Node.js).

## Table of Contents

- [Introduction](#introduction)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [API Endpoints](#api-endpoints)
- [Technologies](#technologies)
- [Contributing](#contributing)
- [License](#license)

## Introduction

This SNS app allows users to create an account, log in, create posts, follow other users, and interact with posts by liking and commenting. It is built using the MERN stack to provide a robust, full-stack JavaScript solution.

## Features

- User authentication (Sign Up, Login)
- Create, read, update, and delete posts
- Like and comment on posts
- Follow and unfollow users
- User profile pages
- News feed showing posts from followed users

## Installation

### Prerequisites

Make sure you have the following installed:

- Node.js
- MongoDB
- npm or yarn

### Steps

1. Clone the repository

    ```sh
    git clone https://github.com/kukutapuvarun/Social-Networking-Service-website.git
    cd sns-app
    ```

2. Install server dependencies

    ```sh
    cd server
    npm install
    ```

3. Install client dependencies

    ```sh
    cd ../client
    npm install
    ```

4. Create a `.env` file in the `server` directory and add the following variables:

    ```env
    MONGO_URI=your_mongodb_connection_string
    JWT_SECRET=your_jwt_secret
    ```

5. Start the server and client

    ```sh
    # In the server directory
    npm start

    # In the client directory
    npm start
    ```

The server will run on `http://localhost:5000` and the client on `http://localhost:3000`.

## Usage

1. Open your browser and navigate to `http://localhost:3000`.
2. Sign up for a new account or log in with an existing account.
3. Start creating posts, following users, and interacting with posts.

## API Endpoints

### Authentication

- `POST /api/auth/signup`: Sign up a new user
- `POST /api/auth/login`: Log in a user

### Posts

- `GET /api/posts`: Get all posts
- `POST /api/posts`: Create a new post
- `GET /api/posts/:id`: Get a specific post
- `PUT /api/posts/:id`: Update a specific post
- `DELETE /api/posts/:id`: Delete a specific post
- `POST /api/posts/:id/like`: Like a post
- `POST /api/posts/:id/comment`: Comment on a post

### Users

- `GET /api/users`: Get all users
- `GET /api/users/:id`: Get a specific user
- `PUT /api/users/:id`: Update a user
- `DELETE /api/users/:id`: Delete a user
- `POST /api/users/:id/follow`: Follow a user
- `POST /api/users/:id/unfollow`: Unfollow a user

## Technologies

- **Frontend**: React, Redux, Axios
- **Backend**: Node.js, Express.js
- **Database**: MongoDB, Mongoose
- **Authentication**: JWT (JSON Web Tokens)
- **Styling**: CSS, Material-UI

## Contributing

Contributions are welcome! Please follow these steps to contribute:

1. Fork the repository
2. Create a new branch (`git checkout -b feature/your-feature`)
3. Commit your changes (`git commit -m 'Add some feature'`)
4. Push to the branch (`git push origin feature/your-feature`)
5. Open a pull request
