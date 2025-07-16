# 📘 Book Management App

A fully functional Book Management App built with **React + Vite**, styled using **Bulma CSS**, and powered by **JSON Server** for API-based data persistence.

Users can:

- ✍️ Add new books
- 🛠️ Edit existing books
- ❌ Delete books
- 📋 View a list of books
- 🖼️ Each book features a random image via [Lorem Picsum](https://picsum.photos)

---

## 🔄 Project Phases

### ✅ Phase 1: Local State Management

- Basic CRUD functionality using React local state (`useState`)
- Books stored temporarily in memory
- No data persistence across refreshes

### ✅ Phase 2: API Integration with JSON Server

- Book data stored and fetched using **JSON Server**
- API requests handled using **Axios**
- All operations (Create, Read, Update, Delete) interact with `http://localhost:3001/books`
- Used **REST Client extension** in VS Code for API testing
- Added additional `useEffect` for syncing and updating local state with server data

### ✅ Phase 3: Centralized State with Context API

- Replaced prop drilling by implementing **React Context API**
- Created centralized `BooksContext` to manage global state and actions
- All components consume book state and actions via `useContext`
- Cleaner component structure and easier state sharing
- Used **`useCallback`** inside context provider to:
  - Avoid stale function references in `useEffect`
  - Optimize functions passed to child components

---

## 🛠️ Tech Stack

- ⚛️ React + Vite
- 🎨 Bulma CSS
- 🧾 Axios for API requests
- 💾 JSON Server (mock backend)
- 🧪 REST Client (for testing API endpoints)
- 🎯 React Hooks: `useState`, `useEffect`, `useContext`, `useCallback`
