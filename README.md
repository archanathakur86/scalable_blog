# Scalable Blog Backend

A Node.js + Express + MongoDB backend for a scalable blog app.

## Features
- JWT authentication
- User registration and login
- CRUD for blog posts
- Ownership checks for update/delete
- Security middleware with Helmet and rate limiting
- Logging with Morgan
- Centralized error handling

## API Routes
- `GET /api/health` - health check
- `POST /api/auth/register` - register user
- `POST /api/auth/login` - login user
- `GET /api/auth/me` - current user profile
- `GET /api/blogs` - list blogs
- `GET /api/blogs/:id` - get single blog
- `POST /api/blogs` - create blog, protected
- `PUT /api/blogs/:id` - update blog, protected
- `DELETE /api/blogs/:id` - delete blog, protected

Legacy alias:
- `GET /api/posts` - same as `/api/blogs`
- `GET /api/posts/:id` - same as `/api/blogs/:id`
- `POST /api/posts` - same as `/api/blogs`, protected
- `PUT /api/posts/:id` - same as `/api/blogs/:id`, protected
- `DELETE /api/posts/:id` - same as `/api/blogs/:id`, protected

## Setup
1. Copy `.env.example` to `.env`
2. Set `MONGODB_URI` and `JWT_SECRET`
3. Install dependencies with `npm install`
4. Start the server with `npm run dev`
