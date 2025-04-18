# Greenlight

A REST API for movie database implemented in Golang. The project has multiple endpoints that enables users to view, add, update, and delete movies from its PostgreSQL database.

## Feature

- Protected CRUD endpoint
- PostgreSQL integration
- SQL Migration
- Structured JSON logging
- Rate limiter
- Error handling
- User registration and activation
- User authentication
- Permission based auth
- Graceful shutdown
- Filtering, sorting, and pagination
- CORS support

## Endpoints

| Method | Routes | Description |
|--------|--------|-------------|
| GET | /v1/healthcheck | Show application health and version information
GET | /v1/movies | Show the details of all movies
POST | /v1/movies | Create a new movie
GET | /v1/movies/:id | Show the details of a specific movie
PATCH | /v1/movies/:id | Update the details of a specific movie
DELETE | /v1/movies/:id | Delete a specific movie
POST | /v1/users | Register a new user
PUT | /v1/users/activated | Activate a specific user
PUT | /v1/users/password | Update the password for a specific user
POST | /v1/tokens/authentication | Generate a new authentication token
POST | /v1/tokens/password-reset | Generate a new password-reset token

## Development

Run the project (in development) using:

`go run ./cmd/api`

And check if it's running by accessing: `localhost:4000/v1/healthcheck`