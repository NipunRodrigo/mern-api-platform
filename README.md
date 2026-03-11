# 🌐 Scalable MERN REST API Platform

> Production-grade RESTful API with JWT authentication, supporting **500+ concurrent users** at **99% uptime**

![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=nodedotjs&logoColor=white)
![Express.js](https://img.shields.io/badge/Express.js-000000?style=flat-square&logo=express&logoColor=white)
![MongoDB](https://img.shields.io/badge/MongoDB-4EA94B?style=flat-square&logo=mongodb&logoColor=white)
![React](https://img.shields.io/badge/React-20232A?style=flat-square&logo=react&logoColor=61DAFB)
![Docker](https://img.shields.io/badge/Docker-2CA5E0?style=flat-square&logo=docker&logoColor=white)

---

## 📋 Overview

This project is a full-stack MERN application template demonstrating:
- ✅ Scalable backend architecture
- ✅ Secure JWT-based authentication & authorization
- ✅ RESTful API design with proper HTTP methods and status codes
- ✅ MongoDB with Mongoose ODM
- ✅ React frontend integrated with the API
- ✅ Docker containerization for easy deployment

---

## 🚀 Getting Started

### Prerequisites
- Node.js v18+
- MongoDB (local or Atlas)
- Docker (optional)

### Installation

```bash
# Clone the repo
git clone https://github.com/nipunrodrigo/mern-api-platform.git
cd mern-api-platform

# Install backend dependencies
cd server && npm install

# Install frontend dependencies
cd ../client && npm install
```

### Environment Variables

Create a `.env` file in `/server`:

```env
PORT=5000
MONGO_URI=mongodb://localhost:27017/mernapp
JWT_SECRET=your_super_secret_key
JWT_EXPIRES_IN=7d
NODE_ENV=development
```

### Run the App

```bash
# Run backend (from /server)
npm run dev

# Run frontend (from /client)
npm start
```

### Docker

```bash
docker-compose up --build
```

---

## 🗂️ Project Structure

```
mern-api-platform/
├── server/
│   ├── config/
│   │   └── db.js
│   ├── controllers/
│   │   ├── authController.js
│   │   └── userController.js
│   ├── middleware/
│   │   ├── authMiddleware.js
│   │   └── errorHandler.js
│   ├── models/
│   │   └── User.js
│   ├── routes/
│   │   ├── authRoutes.js
│   │   └── userRoutes.js
│   └── server.js
├── client/
│   ├── src/
│   │   ├── components/
│   │   ├── pages/
│   │   ├── services/
│   │   └── App.js
│   └── package.json
├── docker-compose.yml
└── README.md
```

---

## 🔐 API Endpoints

| Method | Endpoint | Description | Auth |
|--------|----------|-------------|------|
| POST | `/api/auth/register` | Register new user | ❌ |
| POST | `/api/auth/login` | Login & get token | ❌ |
| GET | `/api/users/profile` | Get user profile | ✅ |
| PUT | `/api/users/profile` | Update profile | ✅ |
| DELETE | `/api/users/:id` | Delete user | ✅ Admin |

---

## 🧪 Testing

```bash
# Run tests
npm test

# With coverage
npm run test:coverage
```

---

## 📄 License

MIT License — feel free to use and contribute!

---

<div align="center">Made with ❤️ by <a href="https://github.com/nipunrodrigo">Nipun Rodrigo</a> | Tampere, Finland 🇫🇮</div>
