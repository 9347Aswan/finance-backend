# Finance Backend API

## Overview
This project is a backend system for managing financial records with role-based access control.

## Features
- User registration and login (JWT authentication)
- Role-based access (Admin, Analyst, Viewer)
- Financial transaction management
- Dashboard summary (income, expense, balance)

## Tech Stack
- Node.js
- Express.js
- MongoDB
- Mongoose

## API Endpoints

### Auth
- POST /api/auth/register
- POST /api/auth/login

### Transactions
- POST /api/transactions
- GET /api/transactions
- GET /api/transactions/summary

### Protected Route
- GET /api/users/admin-data

## Roles
- Admin: Full access
- Analyst: Create & view transactions
- Viewer: View only

## Setup Instructions
1. Install dependencies:
   npm install

2. Start server:
   node index.js

3. Make sure MongoDB is running locally

## Notes
- JWT is used for authentication
- Middleware is used for role-based access control

## How to Test APIs

Use Thunder Client or Postman.

1. Register a user:
POST /api/auth/register

2. Login:
POST /api/auth/login
→ Copy the token

3. Use token in headers:
Authorization: <your_token>

4. Test APIs:
- GET /api/transactions
- POST /api/transactions
- GET /api/transactions/summary


## API Documentation
Provide links to your API documentation (Swagger, Postman, etc.)
- [Swagger Docs](https://your-docs.example.com)
- [Postman Collection](https://your-api.example.com)

## Endpoints
- `GET /transactions` – List all transactions
- `POST /transactions` – Add a new transaction
- `GET /users` – List all users
