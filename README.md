# Full-Stack Chat App 💬

A real-time chat application built with React, Node.js, Express, Socket.IO, and MongoDB. This app enables users to register, log in, and chat instantly with others online using WebSockets.

---

## Table of Contents 📑

- [Project Overview](#project-overview)  
- [Features](#features)  
- [Technology Stack](#technology-stack)  
- [Installation](#installation)  
- [Usage](#usage)  
- [Folder Structure](#folder-structure)  
- [Environment Variables](#environment-variables)  
- [Contributing](#contributing)  
- [License](#license)  

---

## Project Overview 📝

This Full-Stack Chat App consists of a backend built with Node.js and Express that manages user authentication, message routing, and real-time communication using Socket.IO. The frontend is a React application built with Vite and styled with Tailwind CSS. Users can create accounts, log in, and engage in real-time chat sessions.

---

## Features ✨

- User registration and authentication 🔐  
- Real-time one-on-one and/or group chat powered by Socket.IO ⚡  
- Display of online users 👥  
- Responsive UI with Tailwind CSS 📱  
- Secure password hashing and JWT-based authentication 🔒  
- Real-time updates without page refresh 🔄  

---

## Technology Stack 🛠️

- **Frontend:** React.js, Vite, Tailwind CSS  
- **Backend:** Node.js, Express.js, Socket.IO  
- **Database:** MongoDB  
- **Authentication:** JWT (JSON Web Tokens)  
- **Styling:** Tailwind CSS  
- **Build Tools:** Vite  

---

## Installation 📦

### Prerequisites

- Node.js (v14 or newer)  
- npm or yarn  
- MongoDB instance running locally or via cloud (MongoDB Atlas)  

### Steps

1. Clone the repository  
```
bash
git clone https://github.com/yourusername/fullstack-chat-app.git
cd fullstack-chat-app
```

2. Install backend dependencies
```
bash
cd backend
npm install
```

3. Install frontend dependencies
```
bash
cd ../frontend
npm install
```
4. Create .env files with appropriate environment variables as described below.

5. Start the backend server
```
bash
cd ../backend
npm start
```
6. Start the frontend development server
```
bash
cd ../frontend
npm run dev
```
7. Open your browser at http://localhost:3000 to use the app.

## Usage 🚀

- Register a new account or log in with existing credentials  
- View online users and chat in real-time  
- Open multiple browser windows or devices to test messaging  
- Log out when finished  


## Folder Structure 📁

```
/CHAT-APP
├── backend
│ ├── src
│ │ ├── controllers # Business logic for routes
│ │ ├── middleware # Auth and error handling middleware
│ │ ├── models # Mongoose models (User, Message, etc.)
│ │ ├── routes # Express routes (auth, chat, etc.)
│ │ └── server.js # Entry point for backend server
│ ├── package.json # Backend dependencies and scripts
│ └── package-lock.json
│
├── frontend
│ ├── public # Static assets and index.html
│ ├── src
│ │ ├── components # React components (Chat, Login, etc.)
│ │ ├── context # Context API providers if any
│ │ ├── pages # React pages or views
│ │ ├── App.jsx # Root React component
│ │ └── main.jsx # ReactDOM entry point
│ ├── package.json # Frontend dependencies and scripts
│ ├── vite.config.js # Vite config file
│ ├── tailwind.config.js # Tailwind CSS config
│ ├── postcss.config.js # PostCSS config
│ ├── eslint.config.js # ESLint configuration
│ └── package-lock.json
│
├── .gitignore # Specifies intentionally untracked files to ignore
├── LICENSE # License file 
└── README.md 
```
## Environment Variables ⚙️
Create a .env file in the backend directory with the following variables:

```
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret_key
PORT=5000
```
If your frontend requires environment variables, create .env in the frontend directory accordingly.

---
## Contributing 🤝

Contributions are welcome! To contribute:

1. Fork the repository  
2. Create a new branch (`git checkout -b feature-name`)  
3. Make your changes and commit (`git commit -m 'Add new feature'`)  
4. Push to the branch (`git push origin feature-name`)  
5. Open a pull request for review  

---
## License 📄
This project is licensed under the MIT License. See the LICENSE file for details.
