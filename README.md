# Connectly

A full-stack mini social media platform built for the CodeAlpha Full Stack Development internship.

## Features
- User registration, login and editable profile
- Create text posts and view a community feed
- Like/unlike posts and add comments
- Follow/unfollow other users
- JWT-protected APIs and bcrypt password hashing
- SQLite persistence and responsive UI

## Stack
Node.js, Express, SQLite (better-sqlite3), HTML, CSS and vanilla JavaScript.

## Run locally
```bash
npm install
cp .env.example .env
# Set a long random JWT_SECRET in .env
npm run dev
```
Open http://localhost:3000.

## API
- POST /api/auth/register
- POST /api/auth/login
- GET /api/posts
- POST /api/posts (authentication required)
- POST /api/posts/:id/like
- GET/POST /api/posts/:id/comments
- GET/PUT /api/users/me
- POST /api/users/:id/follow
- GET /api/health

The SQLite database is created automatically in data/app.db. This is an educational project; review and test before production use.
