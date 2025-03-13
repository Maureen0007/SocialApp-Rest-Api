# Social Media REST API

This is a fully functional REST API for a social media platform, built using Node.js, Express, and MongoDB. It allows users to create accounts, post content, follow other users, and interact with posts.

## Features

- User authentication (JWT-based)
- Create, read, update, and delete posts
- Like and comment on posts
- Follow and unfollow users
- Secure password hashing with bcrypt

## Technologies Used

- **Backend:** Node.js, Express.js
- **Database:** MongoDB (Mongoose ODM)
- **Authentication:** JWT (JSON Web Token)
- **Password Hashing:** bcrypt

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/Maureen0007/social-media-api.git
   ```
2. Navigate to the project directory:
   ```bash
   cd social-media-api
   ```
3. Install dependencies:
   ```bash
   npm install
   ```
4. Set up environment variables:
   Create a `.env` file in the root directory and add:
   ```env
   MONGO_URI=your_mongodb_connection_string
   JWT_SECRET=your_jwt_secret
   ```
5. Start the server:
   ```bash
   npm start
   ```

## API Endpoints

### Authentication
- `POST /api/auth/register` - Register a new user
- `POST /api/auth/login` - Login and receive a JWT token

### Users
- `GET /api/users/:id` - Get user profile by ID
- `PUT /api/users/:id` - Update user profile
- `DELETE /api/users/:id` - Delete user account

### Posts
- `POST /api/posts` - Create a new post
- `GET /api/posts` - Get all posts
- `GET /api/posts/:id` - Get a single post
- `PUT /api/posts/:id` - Update a post
- `DELETE /api/posts/:id` - Delete a post

### Interactions
- `PUT /api/posts/:id/like` - Like or unlike a post
- `POST /api/posts/:id/comment` - Add a comment to a post

### Follow System
- `PUT /api/users/:id/follow` - Follow a user
- `PUT /api/users/:id/unfollow` - Unfollow a user

## Deployment
This API is deployed at:
```
https://your-deployed-api-url.com
```

## Contributing
Feel free to fork this repository and submit pull requests. Contributions are always welcome!




