# RBAC System

This is a simple Role-Based Access Control (RBAC) system implemented using Node.js, Express, MongoDB, and JWT.

## Features
- User Registration and Login
- Role-Based Authorization (Admin, User, Moderator)
- JWT Authentication
- Protect routes based on user roles

## Endpoints

### /api/auth/register
- Method: POST
- Data: `username`, `email`, `password`, `role` (Admin, User, Moderator)

### /api/auth/login
- Method: POST
- Data: `email`, `password`
- Response: JWT Token

### /api/users (Admin Only)
- Method: GET
- Fetch all users

### /api/users/:id (Admin Only)
- Method: PUT
- Data: `role`
- Update user role

## How to Run
1. Clone the repository
2. Install dependencies: `npm install`
3. Set up `.env` with your MongoDB URI and JWT secret
4. Run the server: `node app.js`
