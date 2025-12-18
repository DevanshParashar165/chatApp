# 💬 Real-Time Chat Application (MERN + Socket.IO)

A full-stack **real-time chat application** built using the **MERN stack** with **Socket.IO** for instant communication.  
The application supports secure authentication, real-time messaging, image sharing, online status tracking, and persistent login.

---

## 🚀 Features

- 🔐 **JWT Authentication**
- 🔄 **Persistent Login on Page Reload**
- 💬 **Real-time 1-to-1 Chat using Socket.IO**
- 🟢 **Online / Offline User Indicator**
- 📸 **Image Messaging (Cloudinary)**
- 👀 **Seen & Unseen Message Handling**
- ⚡ **Instant UI Updates**
- 🛡️ **Protected Routes**
- 🧠 **Optimized State Management using Context API**

---

## 🧑‍💻 Tech Stack

### Frontend
- React.js
- React Router DOM
- Context API
- Axios
- Tailwind CSS
- Socket.IO Client

### Backend
- Node.js
- Express.js
- MongoDB & Mongoose
- Socket.IO
- JWT (JSON Web Token)
- Cloudinary (Image Uploads)

---

---

## 🔐 Authentication Flow

1. User logs in and receives a JWT
2. Token is stored securely and attached to API requests
3. On page reload:
   - Frontend calls `/api/auth/check`
   - Backend validates the token
   - User session is restored automatically

---

## 🔄 Real-Time Messaging Flow

1. User sends a message
2. Message is saved in MongoDB
3. Socket.IO emits a `newMessage` event
4. Receiver gets the message instantly
5. UI updates without page refresh

---

## 🧠 Debugging & Optimizations Implemented

- Fixed **authentication logout on refresh**
- Prevented **infinite socket listeners**
- Solved **white screen crashes caused by malformed messages**
- Normalized socket & API message data
- Added defensive rendering to prevent runtime crashes
- Prevented duplicate messages from REST + socket race conditions

---