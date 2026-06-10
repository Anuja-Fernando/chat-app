# 💬 Chat App

A real-time full-stack chat application built with the MERN stack and Socket.io.

🔗 **Live Demo:** [https://chat-app-5-x4gb.onrender.com](https://chat-app-5-x4gb.onrender.com)

---

## ✨ Features

- 🔐 JWT-based authentication (signup, login, logout)
- 💬 Real-time messaging with Socket.io
- 🟢 Online/offline user status
- 🖼️ Image sharing in chat (up to 10MB)
- 🎨 Multiple themes via DaisyUI
- 📱 Fully responsive UI

---

## 🛠️ Tech Stack

**Frontend**
- React 18 + Vite
- Tailwind CSS + DaisyUI
- Zustand (state management)
- Socket.io-client
- React Router DOM
- Axios

**Backend**
- Node.js + Express
- MongoDB + Mongoose
- Socket.io
- JWT + Cookie-based auth
- bcryptjs

---

## 📁 Project Structure

```
chat-app/
├── frontend/        # React + Vite client
│   └── src/
│       ├── components/
│       ├── pages/
│       ├── store/
│       └── lib/
├── backend/         # Express server
│   └── src/
│       ├── routes/
│       ├── controllers/
│       ├── models/
│       └── lib/
└── package.json
```

---

## 🚀 Run Locally

### Prerequisites
- Node.js v18+
- MongoDB Atlas account

### 1. Clone the repo
```bash
git clone https://github.com/Anuja-Fernando/chat-app.git
cd chat-app
```

### 2. Set up backend environment
Create `backend/.env`:
```env
PORT=5001
MONGODB_URI=your_mongodb_uri
JWT_SECRET=your_jwt_secret
NODE_ENV=development
CLOUDINARY_CLOUD_NAME=your_cloudinary_name
CLOUDINARY_API_KEY=your_cloudinary_key
CLOUDINARY_API_SECRET=your_cloudinary_secret
```

### 3. Install dependencies & run
```bash
# Install backend deps
npm install --prefix backend

# Install frontend deps
npm install --prefix frontend

# Run backend (from root)
npm run dev --prefix backend

# Run frontend (from root)
npm run dev --prefix frontend
```

Frontend runs on `http://localhost:5173`, backend on `http://localhost:5001`.

---

## ☁️ Deployment

Deployed on **Render** as a single web service.

- **Build command:** `npm install --prefix backend && npm install --prefix frontend --include=dev && npm run build --prefix frontend`
- **Start command:** `npm run start`
- **Environment variables:** `NODE_ENV=production`, `MONGODB_URI`, `JWT_SECRET`, etc.

---

## 📄 License

MIT
