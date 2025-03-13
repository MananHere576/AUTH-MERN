# MERN Authentication

This is a **MERN (MongoDB, Express.js, React, Node.js) authentication system**, built for practice purposes. It includes user authentication with secure login and registration functionality.

## Features

- **User Registration & Login** with JWT authentication
- **Password Hashing** using bcrypt
- **Protected Routes** for authenticated users
- **Session Persistence** using local storage
- **Frontend Validation** for user input
- **Role-Based Access Control (RBAC)** (optional enhancement)
- **Email Verification** (optional enhancement)

## Tech Stack

### Frontend:
- React.js
- React Router
- Axios
- Tailwind CSS (for styling)

### Backend:
- Node.js
- Express.js
- MongoDB (Mongoose ODM)
- JWT (JSON Web Token) for authentication
- Bcrypt.js for password hashing
- CORS for handling cross-origin requests

## Installation

### Prerequisites:
- Node.js installed
- MongoDB running (locally or via cloud service like MongoDB Atlas)
- Git installed

### Steps to Run the Project

1. **Clone the repository**
   ```sh
   git clone https://github.com/MananHere576/MERN-Auth.git
   cd MERN-Auth
Backend Setup

sh
Copy
Edit
cd backend
npm install
npm start
Ensure MongoDB is running and configure the .env file with your database URL and JWT secret.

Frontend Setup

sh
Copy
Edit
cd ../frontend
npm install
npm start
Access the Application Open your browser and navigate to:

sh
Copy
Edit
http://localhost:3000
Environment Variables
Create a .env file in the backend directory and add:

sh
Copy
Edit
PORT=5000
MONGO_CONN="your_mongodb_connection_string"
JWT_SECRET="your_jwt_secret"
In the frontend, create a .env file and add:

sh
Copy
Edit
REACT_APP_API_URL=http://localhost:5000
Folder Structure
lua
Copy
Edit
MERN-Auth/
│-- backend/
│   │-- Controllers/
│   │-- Middlewares/
│   │-- Models/
│   │-- Routes/
│   │-- index.js
│   │-- package.json
│   │-- .env (to be configured)
│-- frontend/
│   │-- src/
│   │-- public/
│   │-- package.json
│-- README.md
API Endpoints
Endpoint	Method	Description
/api/auth/signup	POST	Register a new user
/api/auth/login	POST	Authenticate user and return JWT
/api/auth/me	GET	Get user details (protected)
/api/auth/logout	POST	Logout user and clear session
Future Enhancements
OAuth-based login (Google, GitHub, etc.)
Email verification during signup
Multi-factor authentication (MFA)
Password reset functionality
Admin dashboard for user management
Author
Created by Manan for learning and practice purposes. 🚀

Feel free to contribute or provide feedback!
