# SocialMedia Platform (MERN Stack)

A production-grade full-stack social media application developed using the MERN (MongoDB, Express.js, React.js, Node.js) stack. The platform replicates essential social network functionalities such as user authentication, post creation, interactive engagement, and dynamic profile management, backed by a secure and modular API infrastructure.

## Technologies Used

### Backend:
- Node.js with Express.js
- MongoDB with Mongoose ODM
- bcryptjs for password hashing
- jsonwebtoken (JWT) for authentication
- dotenv for environment management
- CORS for cross-origin resource handling

### Frontend:
- React.js (Functional Components with Hooks)
- Axios for HTTP requests
- React Router DOM for SPA routing

## Core Features

- JWT-based user authentication and session management
- Encrypted user credentials using bcrypt
- Full CRUD operations on user posts
- Like and unlike system for post interaction
- Commenting functionality with validation
- Role-based access to protected routes
- Dynamic user profile rendering
- Modular backend architecture with secure middleware integration

## Project Structure
/client              → React.js frontend
/server              → Node.js backend
/server/models       → Mongoose data models
/server/routes       → API route definitions
/server/middleware   → Authentication and authorization logic

## Getting Started

### Prerequisites:
- Node.js installed (v14 or higher recommended)
- MongoDB instance (local or hosted via MongoDB Atlas)
- `.env` file inside `/server` with the following keys:
- MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret_key

### Setup Instructions

1. Clone the repository:

```bash
git clone https://github.com/gowdaarjun/SocialMedia.git
cd SocialMedia

2.	Install backend dependencies and start the backend:
cd server
npm install
npm start

	3.	Install frontend dependencies and start the frontend:
cd ../client
npm install
npm start

API Endpoints Overview
Method
Endpoint
Description
POST
/api/auth/register
Register a new user
POST
/api/auth/login
Authenticate user credentials
GET
/api/posts
Retrieve all posts
POST
/api/posts
Create a new post
PUT
/api/posts/:id
Update an existing post
DELETE
/api/posts/:id
Delete a post
POST
/api/posts/like/:id
Like or unlike a post
POST
/api/comments/:postId
Add a comment to a post
DELETE
/api/comments/:commentId
Delete a specific comment

Future Enhancements
	•	Real-time chat and notifications using WebSocket or Socket.io
	•	Cloud-based media storage for post attachments
	•	Pagination, search, and filtering for scalability
	•	Role-based access control with user groups and admin panels

Author

Developed and maintained by Arjun Gowda
GitHub: https://github.com/gowdaarjun

