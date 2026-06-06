# ♻️ E-Waste Management System

A web-based **E-Waste Management System** designed to promote responsible electronic waste disposal by enabling efficient collection, monitoring, and management of e-waste through a centralized platform.

---

## 📌 Live Demo
🌍 **Access the App Here**: [https://e-waste-bin-management.onrender.com](https://e-waste-bin-management.onrender.com)

---

## 📖 How It Works (App Flow)

The application provides an intuitive flow for users to responsibly dispose of their e-waste:

1. **Sign Up / Login**: Users start by creating an account using their email and verifying it via OTP, or logging in if they already have an account.
2. **Dashboard Overview**: Upon logging in, users are greeted by a personalized dashboard showing their recycling history and accumulated reward points.
3. **Find a Bin**: Users can use the "Find Bin" feature to locate the nearest e-waste collection bins in their vicinity.
4. **Recycle & Scan**: When dropping off e-waste, users log the details of the items. They can scan a QR code at the bin or enter details manually to verify the deposit.
5. **Earn Rewards**: For every verified e-waste deposit, users earn reward points which reflect on their dashboard, encouraging continuous responsible disposal.

---

## 🚀 How to Use the App

### For General Users:
1. **Visit the Portal**: Click on the [Live Demo Link](https://e-waste-bin-management.onrender.com).
2. **Create an Account**: Navigate to the Sign-Up page, fill in your details, and verify your email.
3. **Locate a Bin**: Click on **Find Bin** in the navigation menu to see where you can drop off your old electronics.
4. **Drop & Log**: Take your e-waste to the bin. Use the **Recycle/Scan** option in the app to record your contribution.
5. **Track Progress**: Check your **Dashboard** to see your total recycled items and the rewards you've earned!

---

## 📌 Problem Statement
Electronic waste (e-waste) is one of the fastest-growing waste streams, causing serious environmental and health hazards. Lack of proper monitoring and management leads to inefficient collection and recycling.

This system aims to **digitize e-waste bin management** and **simplify the collection process**.

---

## 🎯 Objectives
- Promote safe and responsible e-waste disposal
- Enable centralized monitoring of e-waste bins
- Improve efficiency in collection and recycling
- Create awareness about e-waste management

---

## ✨ Features
- 📊 **Dashboard view**: Personalized insights and history for users.
- 🗑️ **E-waste bin tracking**: Locate nearby bins easily.
- 👤 **Secure Authentication**: User signup & login with OTP verification.
- 📝 **Waste submission records**: Keep track of what you've recycled.
- 🎁 **Rewards System**: Incentives for consistent recycling.
- 📦 **Database-backed storage**: Secure and reliable using MongoDB.

---

## 🛠️ Tech Stack

### Frontend
- HTML, CSS, JavaScript
- EJS (Embedded JavaScript Templates)

### Backend
- Node.js
- Express.js

### Database
- MongoDB Atlas

---

## 📂 Project Structure

```text
E-Waste-Bin-Management/
│
├── assets/             # CSS, JS, and image assets
├── Backened/
│   ├── controller/     # Logic for user and web routes
│   ├── models/         # MongoDB schemas (User, Bin, RecycledItems)
│   ├── routes/         # Express routes
│   ├── utils/          # Helper functions (Auth, OTP)
│   ├── cloudConfig.js  # Cloud storage configurations
│   ├── index.js        # Main server entry point
│   └── package.json    # Backend dependencies
│
├── Frontened/          # EJS view templates (Dashboard, Login, Scan, etc.)
│
├── .env                # Environment variables (Ignored in Git)
└── README.md           # Project Documentation
```

---

## 🔐 Authentication & Core Modules

### User Management
- **Signup & Login**: Secure access to the platform.
- **Security**: Passwords are securely hashed using `bcrypt`.
- **Session Handling**: User sessions are maintained using HTTP-only cookies.
- **Verification**: Email-based OTP verification supported via `sendOtp.js`.

### Recycling Records
- Track recycled items per user.
- Store recycling history in MongoDB.
- Display data seamlessly on the dashboard.

### Bin Management
- Display available bins with location-based support to guide users effectively.