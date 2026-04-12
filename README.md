# Contact Manager — Backend

REST API for the Contact Manager app. Handles user authentication and contact management.

**Live:** https://contact-manager-mern-backend.onrender.com

**Frontend repo:** https://github.com/Armaan2022/Contact-Manager-MERN-Frontend

## Tech Stack

- Node.js + Express
- MongoDB + Mongoose
- JSON Web Tokens (JWT)
- bcryptjs

## Features

- User registration and login
- JWT-based authentication
- Create, read, update, and delete contacts

## API Endpoints

| Method | Endpoint | Auth | Description |
|--------|----------|------|-------------|
| POST | `/api/register` | No | Register a new user |
| POST | `/api/login` | No | Login and receive a JWT |
| GET | `/api/me` | Yes | Get logged-in user info |
| GET | `/api/mycontacts` | Yes | Get all contacts for the user |
| POST | `/api/contact` | Yes | Create a new contact |
| PUT | `/api/contact` | Yes | Update a contact |
| GET | `/api/contact/:id` | Yes | Get a single contact |
| DELETE | `/api/delete/:id` | Yes | Delete a contact |

## Local Setup

```bash
git clone https://github.com/Armaan2022/Contact-Manager-MERN-Backend.git
cd Contact-Manager-MERN-Backend
npm install
```

Create `config/config.env`:

```
MONGODB_URL=your_mongodb_atlas_connection_string
JWT_SECRET=your_jwt_secret
```

```bash
npm run dev
```

Server runs on http://localhost:5000
