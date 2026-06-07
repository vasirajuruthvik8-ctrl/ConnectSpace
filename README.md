# CONNECT SPHERE (MERN Stack)

A full-stack LinkedIn-inspired professional networking platform built using MongoDB, Express.js, React.js, and Node.js.

## Features

### Authentication

* User Registration
* User Login
* User Logout
* Password Hashing using bcryptjs

### User Profiles

* Professional Profile Creation
* Headline
* Bio
* Location
* Experience
* Education
* Skills
* Profile Editing

### Professional Networking

* Browse People Directory
* View Other User Profiles
* Profile View Tracking
* Premium Profile Analytics

### Social Feed

* Create Posts
* View Posts Feed
* Like Posts
* Delete Own Posts
* Comment System (In Progress)

### Premium Features

* Profile View Analytics
* See Who Viewed Your Profile
* Premium Membership System

### Upcoming Features

* Connections System
* Premium Upgrade Payment Gateway
* Messaging System
* Notifications
* Profile Pictures Upload
* Advanced Search

---

## Tech Stack

### Frontend

* React.js
* React Router DOM
* Axios
* JavaScript
* CSS

### Backend

* Node.js
* Express.js

### Database

* MongoDB
* Mongoose

### Authentication

* bcryptjs

---

## Project Structure

```bash
client/
│
├── src/
│   ├── pages/
│   ├── components/
│   ├── App.jsx
│   └── main.jsx

server/
│
├── controllers/
├── models/
├── routes/
├── config/
└── server.js
```

---

## Database Models

### User

```javascript
{
  name,
  email,
  password,
  headline,
  bio,
  education,
  experience,
  skills,
  location,
  profileViews,
  isPremium
}
```

### Post

```javascript
{
  userId,
  userName,
  content,
  likes,
  createdAt
}
```

---

## API Endpoints

### Authentication

```http
POST /api/auth/register
POST /api/auth/login
PUT  /api/auth/profile/:id
DELETE /api/auth/profile/:id
```

### Users

```http
GET /api/auth/users
POST /api/auth/profile-view/:id
GET /api/auth/profile-views/:id
```

### Posts

```http
POST /api/posts
GET /api/posts
DELETE /api/posts/:id
PUT /api/posts/:id/like
```

---

## Learning Objectives

This project was built to understand:

* Full Stack Development
* REST APIs
* MERN Architecture
* Authentication & Security
* MongoDB Data Modeling
* React State Management
* Professional Networking Systems
* Social Media Feed Design
* Premium Feature Monetization
* Scalable Application Architecture

---

## Future Roadmap

* Connection Requests
* Mutual Connections
* Post Comments
* Payment Gateway Integration
* Real-Time Messaging
* Notifications
* Search and Filters
* Cloud Deployment
* Microservices Architecture

---

## Author

Built as a MERN Stack learning project focused on understanding how large-scale professional networking platforms like LinkedIn are architected and developed.
