# auth-app


# 🔐 React Auth App

A full-stack authentication application using **React** for the frontend, **Node.js (Express)** for the backend, and **PostgreSQL** as the database.

---

## 🚀 Features

- User registration (sign up)
- User login (sign in)
- Password hashing with bcrypt
- JSON Web Token (JWT) authentication
- Protected routes (frontend & backend)
- PostgreSQL for user data storage
- Secure API communication (CORS, HTTPS-ready)


## 📁 Project Structure

---

```markdown

/my-auth-app
├── backend/          # Node.js + Express server
│   ├── controllers/  # Route logic
│   ├── models/       # Database models (PostgreSQL)
│   ├── routes/       # Auth routes
│   ├── middleware/   # Auth middleware (JWT validation)
│   ├── config/       # DB & environment config
│   └── server.js     # Entry point
│
├── frontend/         # React frontend
│   ├── src/
│   │   ├── pages/     # Login, Signup, Dashboard pages
│   │   ├── components/# Reusable components
│   │   ├── context/   # Auth context/provider
│   │   └── App.js
│   └── package.json
│
├── .gitignore
├── README.md
└── package.json      # Root-level if using concurrently

```

---

## 🛠️ Tech Stack

**Frontend:**
- React
- React Router
- Axios

**Backend:**
- Node.js
- Express.js
- PostgreSQL
- bcrypt for password hashing
- JWT for authentication

---

## 📦 Installation

### 1. Clone the Repo
```bash
git clone https://github.com/your-username/my-auth-app.git
cd my-auth-app
```

### 2. Setup Backend
```bash
cd backend
npm install
cp .env.example .env  # Add DB credentials and JWT secret
npm run dev
```

### 3. Setup Frontend
```bash
cd ../frontend
npm install
npm start
```

---

## ⚙️ Environment Variables

### Backend `.env` file
```env
PORT=5000
DATABASE_URL=postgres://username:password@localhost:5432/dbname
JWT_SECRET=your_super_secret_key
```

---

## 🔒 Security Best Practices

- Store passwords hashed with bcrypt
- Use HTTPS in production
- Store JWTs in HttpOnly cookies (not localStorage for prod)
- Use environment variables for secrets

---
