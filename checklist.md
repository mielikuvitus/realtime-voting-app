# 📊 Real-Time Voting App – Build & Learning Checklist

This is a structured checklist for building a tracker for a real-time voting app using React, Redux, and WebSockets.

---

## ✅ Day 1: Setup, Redux & Local State (3h)

### 🧱 Project Setup

- [x] Create new Vite project with React and TypeScript
- [x] Install dependencies and verify local dev server works

---

### 📚 Learn Redux Toolkit Basics

- [x] Understand what Redux is and why it's useful
- [x] Learn what a "slice" is in Redux Toolkit
- [x] Understand how to dispatch actions and update state
- [x] Learn how to connect components to Redux store using Provider

---

### 📘 JavaScript Referencing Concepts

- [x] Learn how primitive vs object referencing works in JavaScript
- [x] Understand object mutation vs reassignment
- [x] Read about reference equality and how it affects state updates

---

### 💻 Build UI & Redux State

#### 🔹 Redux Setup

- [ ] Install Redux Toolkit and React Redux
- [ ] Create Redux store file
- [ ] Create `pollSlice` with a question and multiple options
- [ ] Provide Redux store to the React app

#### 🔸 UI Implementation

- [ ] Display poll question from Redux state
- [ ] Render multiple options as buttons
- [ ] Show vote count beside each option

#### 🔹 Voting Functionality

- [ ] On button click, dispatch vote action to Redux
- [ ] Update option count in the Redux store
- [ ] Reflect updated state in the UI

---

## ⏳ Day 2: Learn WebSockets + Build Real-Time Sync (5–8h)

### 📚 WebSocket Reading & Research

- [ ] Understand how WebSockets work vs HTTP
- [ ] Learn WebSocket lifecycle: connect → message → close
- [ ] Study how WebSocket clients and servers communicate
- [ ] Learn the concept of broadcasting messages to all clients
- [ ] Optionally explore how Socket.IO simplifies real-time logic

---

### 🛠️ WebSocket Server Setup

- [ ] Set up Node.js server with WebSocket support
- [ ] Maintain in-memory poll state on the server
- [ ] Broadcast updated vote counts to all connected clients

---

### 🔗 Client Integration

- [ ] Connect frontend to WebSocket server
- [ ] Send vote message to server on vote action
- [ ] Listen for poll state updates from the server
- [ ] Dispatch Redux action to update UI based on incoming data

---

### 🧪 Testing & Improvements

- [ ] Handle reconnects gracefully
- [ ] Ensure new clients receive the current poll state on join
- [ ] Prevent rapid repeat votes (optional)
- [ ] Add simple connection status UI

---

## ✅ Completion Criteria

- [ ] Votes update in real time across multiple open clients
- [ ] Redux manages all local state
- [ ] Server manages shared poll state and broadcasts changes
- [ ] Frontend reflects all updates without page reload
