# AI-Moderated Chat App - Login System

This repository contains the authentication system for a real-time AI-moderated chat application. It is built using the **MERN stack** and designed for **local development**.

## Features

- User authentication with **JWT** and **bcrypt** for password hashing
- Session management with **HTTP-only cookies**
- **MongoDB** for user data storage
- Role-based access control (RBAC) *(future)*
- Basic **rate limiting** for security
- API built with **Express.js** (Node.js backend)
- React frontend *(to be implemented later)*

## Tech Stack

| Component  | Technology |
|------------|------------|
| Backend    | Node.js, Express.js |
| Database   | MongoDB (local instance) |
| Auth       | JWT for authentication, bcrypt for password hashing |
| Frontend   | React (to be implemented) |

## Installation

### 1. Clone the repository:
```sh
git clone https://github.com/yourusername/chat-auth-local.git
cd chat-auth-local
```

3. Set up environment variables:
Create a .env file in the backend directory:
```
PORT=5000
MONGO_URI=mongodb://localhost:27017/chat-auth
JWT_SECRET=your_secret_key
```

4. Start the application:
Start the backend:
```
cd backend
npm run dev
```
Start the frontend (if applicable):
```
cd frontend
npm start
```

## Notes
- This project is for local development only and is not configured for deployment.
- A MongoDB instance is required (run mongod locally or use MongoDB Atlas).
- OAuth support (Google, GitHub, etc.) is optional and not yet implemented.
- The frontend is not yet complete but will use React.

## Future Plans
- Implement frontend authentication UI (React)
- Add user roles (e.g., admin, moderator)
- Password reset functionality
- WebSocket support for real-time auth
