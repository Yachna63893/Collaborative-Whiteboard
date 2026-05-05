# Collaborative-Whiteboard
# 🎨 Real-Time Collaborative Whiteboard

A cross-platform **real-time collaborative whiteboard application** that allows multiple users to draw, sketch, write, and communicate simultaneously on a shared canvas.

---

## 🚀 Features

### 🟢 Core Features

* ✏️ Real-time drawing and annotation
* 👥 Multiple users on the same board
* 🔗 Join session via shareable link
* 🧹 Clear canvas functionality
* 💾 Save and load whiteboard sessions

### 🟡 Advanced Features

* 📐 Shapes (circle, rectangle, lines)
* 📝 Sticky notes & text boxes
* 💬 Live chat/comments
* ↩️ Undo / Redo support

### 🔵 Bonus (Innovation)

* 🤖 AI-assisted drawing (Antigravity integration)
* 🧠 Smart diagram suggestions
* 🎯 Auto-clean and organize sketches

---

## 🏗️ Tech Stack

### Frontend

* Antigravity / React (Canvas-based UI)
* WebSocket client (SockJS / STOMP)

### Backend

* Spring Boot
* WebSocket (STOMP Protocol)
* REST APIs

### Database

* PostgreSQL / MySQL

### Optional Tools

* Redis (real-time sync optimization)
* AWS S3 / Cloud Storage (for saving boards)

---

## ⚙️ Dependencies (Spring Boot)

* Spring Web
* Spring WebSocket
* Spring Data JPA
* PostgreSQL / MySQL Driver
* Lombok
* Spring Boot DevTools
* (Optional) Spring Security

---

## 🔄 System Architecture

```
Frontend (Canvas UI)
        │
        ▼
WebSocket (Real-time Events)
        │
        ▼
Spring Boot Backend
   ├── REST APIs (Session Management)
   ├── WebSocket (Broadcast Updates)
   └── Database (Persistence)
```

---

## 🔌 How It Works

1. User creates or joins a whiteboard session
2. A unique session ID is generated
3. Users connect via WebSocket
4. Drawing actions are sent as events
5. Backend broadcasts updates to all users
6. All users see changes in real-time

---

## 📡 WebSocket Endpoint

```
/ws
/topic/board/{sessionId}
```

---

## 📁 Project Structure

```
backend/
 ├── controller/
 ├── service/
 ├── model/
 ├── repository/
 └── config/

frontend/
 ├── components/
 ├── canvas/
 └── websocket/
```

---

## 🧪 API Endpoints (Sample)

### Create Session

```
POST /api/session
```

### Join Session

```
GET /api/session/{id}
```

### Save Board

```
POST /api/save
```

---

## 🛠️ Installation & Setup

### Backend

```bash
git clone <repo-url>
cd backend
mvn clean install
mvn spring-boot:run
```

### Frontend

```bash
cd frontend
npm install
npm start
```

---

## 🎯 Hackathon Strategy

* Focus on **real-time performance**
* Keep UI **simple and clean**
* Add **one standout feature (AI / Antigravity)**

---

## 📊 Judging Criteria Covered

* ✅ Real-Time Collaboration
* ✅ Low Latency Performance
* ✅ Scalable Architecture
* ✅ Feature Completeness
* ✅ Innovation (AI integration)

---

## 🚨 Future Improvements

* Role-based access (Admin/User)
* Export as PDF/Image
* Version history
* Multi-board management

---



## 📜 License

This project is open-source and available under the MIT License.

## ⭐ Acknowledgements

* Spring Boot
* WebSocket (STOMP)
* Open-source canvas libraries

👉 *Built for hackathons, optimized for performance, and designed for real-time collaboration.*
