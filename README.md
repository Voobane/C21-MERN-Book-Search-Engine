# 📚 MERN Book Search Engine

A full-stack book search application built with the MERN stack and refactored to use a GraphQL API with Apollo Server. Users can search millions of books via the Google Books API, create an account, and save their favorite titles to a personal reading list.

---

## 📖 Overview

This project was originally built with a RESTful API and later refactored to use **GraphQL and Apollo Server** — a common real-world migration pattern. It demonstrates how to transition from REST to GraphQL while keeping all existing functionality intact, and how to integrate third-party APIs in a full-stack React application.

---

## ✨ Features

- 🔍 Search millions of books powered by the **Google Books API**
- 🔐 User authentication with **JWT (JSON Web Tokens)**
- 📌 Save books to your personal reading list
- 🗑️ Remove books from your saved list
- 📱 Responsive UI built with **React** and **React Bootstrap**
- ⚡ GraphQL queries and mutations replacing all REST endpoints

---

## 🛠️ Tech Stack

| Layer      | Technology                            |
| ---------- | ------------------------------------- |
| Frontend   | React, React Bootstrap, Apollo Client |
| Backend    | Node.js, Express.js, Apollo Server    |
| Database   | MongoDB, Mongoose ODM                 |
| API        | Google Books API                      |
| Auth       | JWT (JSON Web Tokens), bcrypt         |
| Deployment | Render                                |

---

## 🚀 Getting Started

### Prerequisites

- Node.js (v18+)
- MongoDB (local or Atlas cloud instance)
- A Google Books API key (optional for extended quota)

### Installation

```bash
# Clone the repository
git clone https://github.com/Voobane/C21-MERN-Book-Search-Engine.git
cd C21-MERN-Book-Search-Engine

# Install dependencies for both client and server
npm install
cd client && npm install
cd ../server && npm install
```

### Environment Variables

Create a `.env` file in the `/server` directory:

```
MONGODB_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret_key
```

### Running the App

```bash
# From the root — runs both client and server concurrently
npm run develop
```

Visit `http://localhost:3000` in your browser.

---

## 📁 Project Structure

```
C21-MERN-Book-Search-Engine/
├── client/                  # React frontend
│   └── src/
│       ├── components/      # Navbar, SearchBooks, SavedBooks
│       ├── pages/           # Main page views
│       └── utils/           # Apollo queries, mutations, auth helpers
├── server/                  # Express + Apollo Server backend
│   ├── models/              # Mongoose User and Book schemas
│   ├── schemas/             # GraphQL typeDefs and resolvers
│   └── utils/               # JWT auth middleware
└── readme-assets/           # Screenshots
```

---

## 💡 What I Learned

- How to swap a REST API for **GraphQL** using Apollo Server without breaking existing features
- Writing **GraphQL type definitions and resolvers** from scratch
- Using **Apollo Client** on the frontend to replace `fetch` calls with queries and mutations
- Handling **JWT authentication** inside GraphQL context rather than Express middleware
- Deploying a MERN app with separate client/server to **Render**

---

## 📸 Screenshots

> _Add screenshots to the `readme-assets/` folder and update this section._

---

## 👤 Author

**Matt (Voobane)**

- GitHub: [@Voobane](https://github.com/Voobane)
