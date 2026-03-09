# 🌍 Tourism Management & Booking Platform

A full-stack web application for searching, booking tours and hotels, with real-time chat support and an admin dashboard for management and revenue reporting.

This repository contains **two separate implementations** of the same platform using different backend technologies.

---

## 📁 Project Structure

```
tourism-platform/
├── mern/                        # Version 1: MERN Stack
│   ├── backend/                 # Node.js + Express + MongoDB
│   └── frontend/                # React + Vite
│
└── spring-boot/                 # Version 2: Spring Boot Stack
    ├── backend/                 # Spring Boot + MongoDB
    └── frontend/                # React + Vite
```

---

## ✨ Features

### 🔐 Authentication & Account
- User registration and login with JWT authentication
- Secure logout and token management
- Personal profile management (update name, avatar, contact info, change password)

### 🗺️ Tours
- Browse all available tours with detailed information (itinerary, duration, price, images)
- Search tours by keyword, destination, or date
- Filter tours by price range, duration, and category
- Book a tour and select number of participants
- View booking history and booking status

### 🏨 Hotels
- Browse hotels with detailed information (location, amenities, room types, images)
- Search hotels by location, check-in/check-out date, and number of guests
- Filter hotels by price range and amenities
- Book a room and choose room type
- View hotel booking history and status

### 💳 Payment
- Multiple payment methods:  **PayPal**, **Stripe**
- Secure payment processing

### ⭐ Reviews & Ratings
- Write and submit reviews for tours and hotels after booking
- Rate with a star system (1–5 stars)
- View all reviews from other users

### 💬 Real-time Chat
- Live chat directly with **admin/support staff** for travel consultation and booking assistance
- Option to chat with an **AI-powered chatbot** for instant automated responses
- Chat history saved and accessible anytime

### 🛠️ Admin Dashboard
- **Tour Management**: Create, update, delete, and view all tours
- **Hotel Management**: Create, update, delete, and view all hotels
- **Booking Management**: View and update status of tour and hotel bookings
- **User Management**: View registered users and manage accounts
- **Revenue Reports**: Visual charts and statistics on bookings and revenue by period

---

## 🧰 Tech Stack

| Layer      | MERN Version              | Spring Boot Version        |
|------------|---------------------------|----------------------------|
| Frontend   | React + Vite              | React + Vite               |
| Backend    | Node.js + Express         | Spring Boot (Java)         |
| Database   | MongoDB                   | MongoDB                    |
| Real-time  | Socket.IO                 | WebSocket                  |

---

## 🚀 Getting Started

### Prerequisites

- [Node.js](https://nodejs.org/) (v18+)
- [npm](https://www.npmjs.com/) or [yarn](https://yarnpkg.com/)
- [MongoDB](https://www.mongodb.com/) (local or Atlas)
- [Java 17+](https://adoptium.net/) *(Spring Boot version only)*
- [Maven](https://maven.apache.org/) *(Spring Boot version only)*

---

## ▶️ Running the MERN Version

### 1. Backend (Node.js + Express)

```bash
cd mern/backend
npm install
```

Create a `.env` file in `mern/backend/` by copying the provided example file:

```bash
cp mern/backend/.env.example mern/backend/.env
```

Then open `.env` and fill in your own values. See `.env.example` for descriptions of each variable.

Start the backend server:

```bash
npm run dev
```

> Server runs at `http://localhost:3000`

---

### 2. Frontend (React + Vite)

```bash
cd mern/frontend
npm install
npm run dev
```

> App runs at `http://localhost:5173`

---

## ▶️ Running the Spring Boot Version

### 1. Backend (Spring Boot)

```bash
cd spring-boot/backend
```

Create your config file by copying the provided example:

```bash
cp spring-boot/backend/src/main/resources/application.properties.example spring-boot/backend/src/main/resources/application.properties
```

Then open `application.properties` and fill in your own values. See `application.properties.example` for descriptions of each variable.

Build and run:

```bash
mvn spring-boot:run
```

> Server runs at `http://localhost:8080`

---

### 2. Frontend (React + Vite)

```bash
cd spring-boot/frontend
npm install
npm run dev
```

> App runs at `http://localhost:5173`

---

## 🌐 Live Demo

| Version | Demo |
|---------|------|
| MERN (Vagabond) | [https://ie213-p22-nhom17-frontend.onrender.com](https://ie213-p22-nhom17-frontend.onrender.com) |
| Spring Boot | Coming soon |

> ⚠️ **Note:** The backend is hosted on Render's free tier. On the first visit, please allow **30–50 seconds** for the server to wake up before the app becomes fully functional.

---

## 📄 License

This project is licensed under the [MIT License](LICENSE).
