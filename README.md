# RoleCrack Backend ⚙️

[🔗 Live Demo](https://role-crack-frontend.vercel.app/)

This is the **backend** server for the RoleCrack application. It provides RESTful APIs for user authentication, session management, AI-powered Q&A generation, and MongoDB-based data persistence.

## 🚀 Key Features

- 🔐 **User Authentication** – Register/login using JWT-based authentication.
- 🤖 **AI Integration (Gemini API)** – Auto-generate Q&A and on-demand concept explanations.
- 🗃️ **MongoDB Storage** – Store user data, sessions, questions.
- 📌 **Question Pinning API** – Pin/unpin questions for better organization.
- 📚 **RESTful APIs** – Modular endpoints for users, sessions, questions, and AI.

## 🛠️ Tech Stack

- Node.js
- Express.js
- MongoDB + Mongoose
- JWT Authentication
- Gemini AI API (via Google API or similar)
- CORS, dotenv, body-parser

## 🔧 Getting Started

### 1. Prerequisites

- Node.js
- MongoDB Atlas account
- Gemini API Key

### 2. Installation

```bash
git clone https://github.com/agprateek7/RoleCrack-backend.git
cd rolecrack-backend
npm install
```

### 3. Environment Variables

Create a `.env` file in the root:

```env
PORT=5000
MONGO_URI=your_mongo_connection_string
JWT_SECRET=your_jwt_secret
GEMINI_API_KEY=your_gemini_api_key
```

### 4. Running the Server

```bash
node server.js
```

Server will run at `http://localhost:5000`.

## 📁 Project Structure

```
src/
├── controllers/         # Handles logic for each API
├── models/              # Mongoose models (User, Session, Question)
├── routes/              # Route definitions
├── middleware/          # JWT auth middleware
├── utils/               # Helper functions, Gemini API integration
├── uploads/             # For storing user profile images
└── server.js             # Entry point
```

## 🔌 API Endpoints

### 🔐 Auth

- `POST /api/auth/register`  
- `POST /api/auth/login`  
- `GET /api/auth/profile`

### 📁 Sessions

- `POST /api/sessions/create`  
- `GET /api/sessions/my-sessions`  
- `GET /api/sessions/:id`  
- `DELETE /api/sessions/:id`

### 🧠 Questions

- `POST /api/questions/add`  
- `PATCH /api/questions/:id/pin`
- `PATCH /api/questions/:id/note`

### 🤖 AI

- `POST /api/ai/generate-questions`  
- `POST /api/ai/generate-explanation`

## 🔗 Frontend Repository

👉 [RoleCrack Frontend](https://github.com/agprateek7/RoleCrack-frontend)

## 📄 License

This project is licensed under the **MIT License**.
# RoleCrack Backend ⚙️

[🔗 Live Demo](https://role-crack-frontend.vercel.app/)

This is the **backend** server for the RoleCrack application. It provides RESTful APIs for user authentication, session management, AI-powered Q&A generation, and MongoDB-based data persistence.

## 🚀 Key Features

- 🔐 **User Authentication** – Register/login using JWT-based authentication.
- 🤖 **AI Integration (Gemini API)** – Auto-generate Q&A and on-demand concept explanations.
- 🗃️ **MongoDB Storage** – Store user data, sessions, questions.
- 📌 **Question Pinning API** – Pin/unpin questions for better organization.
- 📚 **RESTful APIs** – Modular endpoints for users, sessions, questions, and AI.

## 🛠️ Tech Stack

- Node.js
- Express.js
- MongoDB + Mongoose
- JWT Authentication
- Gemini AI API (via Google API or similar)
- CORS, dotenv, body-parser

## 🔧 Getting Started

### 1. Prerequisites

- Node.js
- MongoDB Atlas account
- Gemini API Key

### 2. Installation

```bash
git clone https://github.com/agprateek7/RoleCrack-backend.git
cd rolecrack-backend
npm install
```

### 3. Environment Variables

Create a `.env` file in the root:

```env
PORT=5000
MONGO_URI=your_mongo_connection_string
JWT_SECRET=your_jwt_secret
GEMINI_API_KEY=your_gemini_api_key
```

### 4. Running the Server

```bash
node server.js
```

Server will run at `http://localhost:5000`.

## 📁 Project Structure

```
src/
├── controllers/         # Handles logic for each API
├── models/              # Mongoose models (User, Session, Question)
├── routes/              # Route definitions
├── middleware/          # JWT auth middleware
├── utils/               # Helper functions, Gemini API integration
├── uploads/             # For storing user profile images
└── server.js             # Entry point
```

## 🔌 API Endpoints

### 🔐 Auth

- `POST /api/auth/signup`  
- `POST /api/auth/login`  
- `GET /api/auth/profile`

### 📁 Sessions

- `POST /api/sessions`  
- `GET /api/sessions`  
- `GET /api/sessions/:id`  
- `DELETE /api/sessions/:id`

### 🧠 Questions

- `POST /api/questions/add`  
- `PATCH /api/questions/pin/:id`

### 🤖 AI

- `POST /api/ai/generate-interview`  
- `POST /api/ai/explain`

## 🔗 Frontend Repository

👉 [RoleCrack Frontend](https://github.com/agprateek7/RoleCrack-frontend)

## 📄 License

This project is licensed under the **MIT License**.