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

```text
Role-based-authorization/
├── src/
│   ├── controllers/
│   │   ├── auth.controller.js
│   │   └── music.controller.js
│   ├── db/
│   │   └── db.js
│   ├── middlewares/
│   │   └── auth.middleware.js
│   ├── models/
│   │   ├── album.model.js
│   │   ├── music.model.js
│   │   └── user.model.js
│   ├── routes/
│   │   ├── auth.routes.js
│   │   └── music.routes.js
│   ├── services/
│   │   └── storage.service.js
│   └── app.js
├── .env.example
├── .gitignore
├── package.json
├── package-lock.json
├── README.md
└── server.js
```
