# ✨ Full Stack Realtime Chat App ✨
A modern fullstack chat application built with **React**, **Vite**, **Zustand**, **Tailwind CSS** (frontend) and **Node.js**, **Express**, **MongoDB**, **Mongoose** (backend).  
Supports real-time messaging, group chats, authentication, and profile management.

---

## Features

- User authentication (signup, login, logout)
- Realtime messaging (direct and group)
- Group chat creation and management
- Online users indicator
- Profile page with avatar upload
- Responsive UI with Tailwind CSS & DaisyUI
- Image attachments in chat
- Search users and groups
- Toast notifications for actions

---

## Tech Stack

### Frontend

- [React](https://react.dev/)
- [Vite](https://vitejs.dev/)
- [Zustand](https://zustand-demo.pmnd.rs/)
- [Tailwind CSS](https://tailwindcss.com/)
- [DaisyUI](https://daisyui.com/)
- [React Hot Toast](https://react-hot-toast.com/)
- [Lucide Icons](https://lucide.dev/icons/)

### Backend
https://wishpr.onrender.com
- [Node.js](https://nodejs.org/)
- [Express](https://expressjs.com/)
- [MongoDB](https://www.mongodb.com/)
- [Mongoose](https://mongoosejs.com/)
- [Cloudinary](https://cloudinary.com/) (for image uploads)
- [Socket.io](https://socket.io/) (for realtime features)
- [bcryptjs](https://www.npmjs.com/package/bcryptjs) (for password hashing)
- [dotenv](https://www.npmjs.com/package/dotenv) (for environment variables)

---

## Folder Structure

```
fullstack-chat-app/
├── backend/
│   ├── src/
│   │   ├── controllers/
│   │   ├── lib/
│   │   ├── middleware/
│   │   ├── models/
│   │   ├── routes/
│   │   ├── seeds/
│   │   └── index.js
│   ├── .env
│   └── package.json
├── frontend/
│   ├── src/
│   │   ├── components/
│   │   ├── constants/
│   │   ├── lib/
│   │   ├── pages/
│   │   ├── store/
│   │   ├── App.jsx
│   │   ├── main.jsx
│   │   └── index.css
│   ├── public/
│   ├── index.html
│   ├── package.json
│   ├── tailwind.config.js
│   └── vite.config.js
```

---

## Getting Started

### Prerequisites

- Node.js (v18+ recommended)
- npm or yarn
- MongoDB instance (local or [MongoDB Atlas](https://www.mongodb.com/cloud/atlas))

---

### 1. To main dir

```bash
cd fullstack-chat-app
```

---

### 2. Setup Backend

```bash
cd backend
npm install
```

- Create a `.env` file in `backend/` with the following (edit as needed):

  ```
  PORT=5001
  MONGO_URI=your_mongodb_connection_string
  JWT_SECRET=your_jwt_secret
  CLOUDINARY_CLOUD_NAME=your_cloudinary_name
  CLOUDINARY_API_KEY=your_cloudinary_key
  CLOUDINARY_API_SECRET=your_cloudinary_secret
  ```

- Start the backend server:

  ```bash
  npm run dev
  ```

---

### 3. Setup Frontend

```bash
cd ../frontend
npm install
```

- The frontend is configured to proxy API requests to the backend (`vite.config.js`).
- Start the frontend dev server:

  ```bash
  npm run dev
  ```

- Visit [http://localhost:5173](http://localhost:5173) in your browser.

---

## Usage

- **Sign up** for a new account or **log in** with existing credentials.
- **Start a chat** with any user or create a **group chat**.
- **Send messages** (text or images) in real time.
- **Update your profile** from the profile page.

---

## Environment Variables

See `.env.example` in the backend for all required environment variables.

---

## Credits

- [RandomUser.me](https://randomuser.me/) for demo avatars
- [Cloudinary](https://cloudinary.com/) for image hosting

---


## Troubleshooting

- Make sure both backend and frontend servers are running.
- Check your `.env` configuration.
- If you change backend ports, update the proxy in `frontend/vite.config.js`.

---

## Contributing

Pull requests are welcome! For major changes, please open an issue first to discuss what you would like to change.
