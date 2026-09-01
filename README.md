# 🎟️ Eventora — Frontend

Eventora is a modern and responsive **event booking platform frontend** built with React.js, Vite, and Tailwind CSS. It provides users with an intuitive interface to discover events, authenticate securely, verify bookings using OTP, manage bookings, and access personalized dashboards.

---

## 🌐 Live Demo

- 🎨 Frontend: https://eventora-frontend-alpha.vercel.app/
- ⚙️ Backend API: https://eventora-backend-70xp.onrender.com/

---

## ✨ Features

### 🔐 Authentication

* User registration and login
* JWT-based authentication
* Email OTP verification
* Secure authentication state management
* Persistent login using browser local storage
* Logout functionality

### 📅 Event Discovery

* Browse available events
* View detailed event information
* Event categories
* Event dates and descriptions
* Event images
* Free and paid event support
* Real-time seat availability

### 🎫 Booking Management

* Submit event booking requests
* OTP verification before completing bookings
* View booking status
* Track pending and confirmed bookings
* Cancel eligible bookings
* Payment status visibility

### 👨‍💼 Admin Dashboard

Authorized administrators can access the admin dashboard to:

* Create events
* Update events
* Delete events
* Review booking requests
* Approve or reject bookings
* Manage payment status
* Monitor event statistics
* View revenue and booking analytics

### 🎨 UI/UX

* Responsive design
* Modern and clean interface
* Tailwind CSS styling
* Interactive components
* Micro-interactions
* Mobile-friendly layouts
* Intuitive navigation

---

## 🛠️ Tech Stack

| Technology      | Purpose                  |
| --------------- | ------------------------ |
| ⚛️ React.js     | Frontend UI              |
| ⚡ Vite          | Development & build tool |
| 🎨 Tailwind CSS | Styling                  |
| 🌐 Axios        | API communication        |
| 🔀 React Router | Client-side routing      |
| 🔐 JWT          | Authentication           |
| 📦 npm          | Package management       |
| 🚀 Vercel       | Deployment               |

---

## 🏗️ Project Structure

```text
Eventora-Frontend/
│
├── public/
│   └── favicon.svg
│
├── src/
│   ├── assets/
│   ├── components/
│   ├── context/
│   ├── pages/
│   ├── utils/
│   ├── App.jsx
│   └── main.jsx
│
├── .gitignore
├── index.html
├── package.json
├── package-lock.json
├── vite.config.js
└── README.md
```

---

## 🔄 Application Flow

```text
👤 User
   │
   ├── Register
   │      ↓
   │   📧 Email OTP
   │      ↓
   │   Account Activated
   │
   ├── Login
   │      ↓
   │   🔐 Authentication
   │
   ├── Browse Events
   │      ↓
   │   🎫 Select Event
   │      ↓
   │   📧 Booking OTP
   │      ↓
   │   Booking Request
   │      ↓
   │   ⏳ Pending
   │
   └──────────────────┐
                      ↓
               👨‍💼 Admin Dashboard
                      │
                ┌─────┴─────┐
                ↓             ↓
             Approve       Reject
                │
                ↓
        🎟️ Booking Confirmed
                │
                ↓
          📧 Email Notification
```

---

## ⚙️ Installation & Setup

### 📋 Prerequisites

Make sure you have installed:

* Node.js
* npm
* Git

### 1️⃣ Clone Repository

```bash
git clone https://github.com/OmPimple26/Eventora-Frontend.git
cd Eventora-Frontend
```

### 2️⃣ Install Dependencies

```bash
npm install
```

### 3️⃣ Configure Environment Variables

Create a `.env` file in the project root:

```env
VITE_API_URL=http://localhost:5000/api
```

For production, configure the deployed backend URL:

```env
VITE_API_URL=https://eventora-backend-70xp.onrender.com/api
```

> ⚠️ **Important:** Never commit `.env` files containing sensitive configuration to GitHub.

### 4️⃣ Start Development Server

```bash
npm run dev
```

The application will typically run at:

```text
http://localhost:5173
```

---

## 🔗 Backend Integration

The frontend communicates with the Eventora REST API using **Axios**.

```text
React Frontend
      │
      │ Axios
      ▼
Eventora REST API
      │
      ▼
MongoDB Atlas
```

### Backend API

⚙️ `https://eventora-backend-70xp.onrender.com`

The frontend uses the `VITE_API_URL` environment variable to configure the backend API endpoint.

---

## 🔑 Demo Admin Access

The Admin Dashboard is restricted to authorized administrator accounts.

**Demo credentials:**

```text
Email:    admin@eventora.com
Password: password123
```

> ⚠️ These credentials are provided for demonstration and testing purposes only. Do not use them for production systems.

---

## 📱 Responsive Design

Eventora's frontend is designed to work across:

* 💻 Desktop
* 💻 Laptop
* 📱 Mobile
* 📟 Tablet

---

## 🚀 Deployment

The frontend is deployed using **Vercel**.

### Production Build

```bash
npm run build
```

This generates the production build inside:

```text
dist/
```

### Preview Production Build

```bash
npm run preview
```

---

## 🔒 Security Considerations

* JWT tokens are handled through authenticated API requests.
* Protected routes restrict unauthorized access.
* Admin functionality is controlled through backend authorization.
* Environment variables are used for configurable API endpoints.
* Sensitive credentials are excluded from version control.

> **Note:** Client-side access restrictions should not be considered sufficient security. Authorization is enforced by the backend API.

---

## 📌 Future Enhancements

* 💳 Online payment gateway integration
* 🎟️ QR-code ticket generation
* 🔔 Real-time notifications
* 🔎 Advanced event search and filtering
* ⭐ Event ratings and reviews
* 📱 Progressive Web App (PWA) support
* 🌙 Dark mode

---

## 👨‍💻 Author

**Om Pimple**

B.Tech Computer Engineering | Full-Stack Developer

---

## ⭐ Support

If you find Eventora useful or interesting, consider giving the repository a ⭐ **Star** on GitHub!
