# Role-Based Music API

A Node.js and Express REST API for a music platform with separate access for users and artists. Users can browse music and albums. Artists can upload music to ImageKit and create albums.

## Features

- User registration, login, and logout
- Password hashing with bcrypt
- JWT authentication stored in an HTTP cookie
- Role-based access for `user` and `artist`
- Artist-only music upload and album creation
- Browse music and albums
- MongoDB data storage with Mongoose
- Music file uploads through ImageKit

## Tech Stack

- Node.js
- Express
- MongoDB and Mongoose
- JSON Web Tokens
- bcryptjs
- Multer
- ImageKit

## Requirements

- Node.js and npm
- A MongoDB connection URI
- An ImageKit private key

## Project Structure
src/
├── controllers/   # Authentication and music request handlers
├── db/            # MongoDB connection
├── middlewares/   # Role and token checks
├── models/        # User, music, and album schemas
├── routes/        # API route definitions
└── services/      # ImageKit upload service
server.js          # Loads environment variables and starts the server
