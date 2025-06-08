# 🧠 Post-It Blog App - Backend

This is the backend Repo for the **Post-It Blog App**, a full-stack blogging application built with the MERN stack. It handles user authentication using JWT, password hashing with bcrypt, and CRUD operations for blog posts.

## 🛠️ Tech Stack
- Node.js
- Express.js
- MongoDB (Mongoose)
- JWT Authentication
- Bcrypt for password hashing

## 📦 Features
- User registration and login
- JWT-based authentication
- CRUD operations on blog posts (Create, Read, Update, Delete)
- Authorization: Only post authors can update or delete their posts

## 📁 API Routes

### 🔐 Auth Routes
- `POST /api/register` - Register a new user
- `POST /api/login` - Log in and receive a JWT token

### 📄 Blog Post Routes
- `GET /api/posts` - Get all blog posts
- `POST /api/posts` - Create a new blog post (Protected)
- `PUT /api/posts/:id` - Update a blog post (Protected)
- `DELETE /api/posts/:id` - Delete a blog post (Protected)

## 🧪 Tools & Libraries
- `dotenv` - Environment variable management
- `jsonwebtoken` - Token-based authentication
- `bcrypt` - Secure password hashing
- `cors` - Cross-origin resource sharing
- `mongoose` - MongoDB object modeling

## 📁 Folder Structure
<pre>
post-it-blog-app-backend/
├── controllers/
│   ├── auth.controller.js
│   └── post.controller.js
├── models/
│   ├── User.js
│   └── Post.js
├── routes/
│   ├── auth.js
│   └── posts.js
├── middleware/
│   └── auth.js
├── config/
│   └── db.js
├── .env
├── server.js
</pre>

## 📝 Setup Instructions
```bash
git clone https://github.com/jeevan42/post-it-blog-app-backend
cd post-it-blog-app-backend
npm install
# Add .env file with your MongoDB URI and JWT_SECRET
npm start
```

## 🙌 Contributing
PRs and stars are welcome. For major changes, open an issue first to discuss what you would like to change.
