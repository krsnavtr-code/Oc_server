# Server (Node.js + Express)

This is the **server-side** of the project, built with Node.js, Express, and MongoDB (via Mongoose).

## Features
- RESTful API endpoints
- User authentication (signup route example)
- JWT-based authentication
- MongoDB integration (Mongoose)
- Environment variable support with dotenv
- CORS enabled

## Getting Started

### Prerequisites
- Node.js (v18 or later recommended)
- npm
- MongoDB database (Atlas or local)

### Setup
1. Clone the repository and navigate to the `server` directory:
   ```bash
   cd server
   npm install
   ```
2. Create a `.env` file in the `server` directory:
   ```env
   PORT=5000
   MONGO_URI=your_mongodb_connection_string
   JWT_SECRET=yourSecretKey
   ```

### Running in Development
```bash
npm run dev
```
- Starts the server with nodemon for auto-reloading.
- Default port: 5000

### Running in Production
```bash
npm start
```

## Scripts
- `dev`: Start with nodemon (development)
- `start`: Start with Node.js (production)

## Folder Structure
- `routes/` - Express route handlers (e.g., `auth.js`)
- `controllers/` - Route controller logic
- `models/` - Mongoose models (e.g., `User.js`)
- `index.js` - Main server entry point

## Environment Variables
- `PORT`: Port to run the server on (default: 5000)
- `MONGO_URI`: MongoDB connection string
- `JWT_SECRET`: Secret key for JWT authentication

## Dependencies
- express, mongoose, cors, dotenv, bcryptjs, jsonwebtoken

## Dev Dependencies
- nodemon

## Notes
- Ensure MongoDB URI and JWT secret are set in `.env` before starting.
- The server uses ES module syntax (`import/export`).
- API endpoints are available at `/api/...` (see routes).
