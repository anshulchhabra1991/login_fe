# login_fe - User Authentication App

This is a simple login and signup web application built with React, Vite, and Axios. It allows users to sign up, sign in, and be redirected based on the response from the backend server.

## Features

- User can sign up with name, email, and password.
- User can sign in with email and password.
- API requests are made to a backend server for authentication.
- Toast notifications for success/error messages.
- Conditional redirects based on API response (after successful sign-in, user is redirected to the home page).
- Error handling for invalid credentials and network issues.

## Project Setup

### 1. Clone the repository

Clone the repository using the following command:

```bash
git clone https://github.com/anshulchhabra1991/login_fe.git
```

### 2. Install Dependencies

Navigate to the project folder and install dependencies:

```bash
cd login_fe
npm install
```

### 3.Start the Application

Run the application in development mode using:

```bash
npm run dev
```
The app will be available at http://localhost:3000.


### 4. Build the Application

To create a production-ready build of the application, run:

```bash
npm run build
```
The built files will be available in the dist/ folder.


## API Endpoints

This app interacts with a backend API (e.g., built with NestJS). Below are the key endpoints:

## POST /auth/signup
Request body:
```bash
{
  "name": "John Doe",
  "email": "john.doe@example.com",
  "password": "password123"
}
```
Response:
```bash
{
  "status": true,
  "message": "Sign up successful!"
}
```

## POST /auth/signin
Request body:
```bash
{
  "email": "john.doe@example.com",
  "password": "password123"
}
```
Response:
```bash
{
  "status": true,
  "message": "Sign in successful!"
}
```

## Toast Notifications
```bash
- On success (e.g., successful sign-in), a success toast notification is shown.
- On failure (e.g., invalid credentials), an error toast notification is shown.
```

## Built With
```bash
React - JavaScript library for building user interfaces.
Vite - Next-generation, fast, and optimized build tool for front-end development.
Axios - Promise-based HTTP client for the browser and Node.js.
React Router - A library for handling navigation in React applications.
```