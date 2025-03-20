# Image Management Application Backend

## 📌 Project Overview

This project is a secure back-end system for managing images with user authentication and role-based access control (RBAC). It allows users to upload, store, retrieve, and manage images efficiently.

## 🚀 Features

User Authentication & Security: Implemented JWT-based authentication with password hashing using Bcrypt.

Secure Image Uploads: Used Cloudinary & Multer for secure image storage and retrieval.

Data Management: Integrated search, sorting, and pagination for efficient image retrieval.

Role-Based Access Control: Restricted access to admin routes with authentication and authorization middlewares.

Error Handling & Security: Ensured proper error handling and secured environment variables using dotenv.

## 🛠️ Tech Stack

Back-end: Node.js, Express.js

Database: MongoDB

Authentication: JWT, Bcrypt

File Upload: Multer, Cloudinary

API Testing: Postman

API Endpoints

### Authentication Routes (/api/auth)
Method  Endpoint          Description
POST    /register         Register a new user
POST    /login            Login user & generate JWT
PUT     /change-password  Change user password (Authenticated)


### Home Route (/api/home)
Method  Endpoint   Description
GET     /home      Welcome message for authenticated users


### Admin Route (/api/admin)
Method    Endpoint   Description
GET       /admin     Admin dashboard (Restricted to admin users)

### Image Management Routes (/api/image)
Method  Endpoint           Description  
POST    /upload/image      Upload an image (Admin Only)
GET     /get/images        Retrieve all images (Authenticated)
DELETE  /delete-image/:id  Delete an image (Admin Only)

### Challenges Faced & Learnings
Secure File Uploads: Ensured secure handling of image files using Multer and Cloudinary, preventing malicious uploads.
Optimized Database Queries: Improved search and pagination for efficient data retrieval in MongoDB.
Authentication & Authorization: Implemented JWT authentication and role-based access to protect sensitive endpoints.

### Setup Instructions
Clone the Repository: `git@github.com:narendrajethi220/Image-Management-Application-Backend.git`
Install Dependencies: npm install
Set Up Environment Variables: (Create a .env file)
Run the Server: nodemon start server

Test API Endpoints Using Postman

### Future Enhancements
Implement image categorization and tagging.
Add user activity logging for security.
Optimize performance with caching mechanisms.

#### Developed with ❤️ by Narendra Singh Jethi.
