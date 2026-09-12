# Task Management API

RESTful API built with Node.js, Express, and MongoDB for managing tasks. Includes CRUD operations, title filtering, and Newman-verified testing.

## Tech Stack
- Node.js
- Express
- MongoDB Atlas (Mongoose)

## Environment Variables
Create a .env file in the root directory:

PORT=5000
MONGO_URI=your_mongodb_connection_string

## Setup and Running
npm install
node server.js

## Endpoints
- POST /api/tasks: Create a new task
- GET /api/tasks: Retrieve all tasks
- GET /api/tasks?title=x: Filter tasks by title
- GET /api/tasks/:id: Retrieve task by ID
- PUT /api/tasks/:id: Update task by ID
- DELETE /api/tasks/:id: Delete task by ID

## Testing
Postman collection included in root: Task_API_Collection.postman_json

Run tests via Newman:
npx newman run Task_API_Collection.postman_json
