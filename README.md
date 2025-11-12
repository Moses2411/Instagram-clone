# Instagram Clone API

A backend replica of Instagram built with FastAPI, implementing core social media functionalities with user authentication, posts, comments, and image uploads.

## Features
- User registration and JWT authentication
- Create, read, update, and delete posts
- Comment system on posts
- Image upload functionality
- User profile management
- RESTful API with proper documentation

## Tech Stack
- Backend Framework: FastAPI
- Database: PostgreSQL
- ORM: SQLAlchemy
- Authentication: JWT Tokens
- File Upload: Python-multipart

## API Endpoints

### Authentication
- POST /auth/register - User registration
- POST /auth/login - User login with JWT token
- POST /auth/verify-email - Email verification

### Posts
- POST /posts/ - Create a new post with image upload
- GET /posts/ - Get all posts with pagination
- GET /posts/{post_id} - Get specific post details
- PUT /posts/{post_id} - Update a post
- DELETE /posts/{post_id} - Delete a post

### Comments
- POST /posts/{post_id}/comments - Add comment to a post
- GET /posts/{post_id}/comments - Get all comments for a post
- DELETE /comments/{comment_id} - Delete a comment

### Users
- GET /users/ - Get all users
- GET /users/{user_id} - Get specific user profile
- PUT /users/{user_id} - Update user profile

## Project Structure
