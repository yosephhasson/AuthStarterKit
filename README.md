# Firebase Auth Starter Kit

A reusable authentication starter built with Firebase Authentication.  
This project provides a clean foundation for implementing user authentication in modern applications, including email/password and third-party providers.

---

## 🚀 Overview

This boilerplate is designed to accelerate development by providing a ready-to-use authentication layer powered by Firebase.

It includes:

- User registration and login
- Firebase Authentication integration
- Clean structure for scaling into production apps
- Easy extensibility for additional providers (Google, Apple, etc.)

Firebase Authentication allows you to manage authentication without building your own backend, supporting multiple providers out of the box.  

---

## ✨ Features

- 🔐 Email & Password Authentication
- 🔄 Persistent user sessions
- 🚪 Login / Logout flow
- ⚡ Firebase SDK integration
- 🧱 Modular and scalable structure
- 🧪 Ready for expansion (Google, Apple, Phone auth, etc.)

---

## 🏗️ Project Structure

```text
firebaseAuth
├── src
│   ├── components       # UI components
│   ├── services         # Firebase config & auth logic
│   ├── screens/pages    # Auth screens (Login/Register)
│   ├── hooks            # Reusable logic (if applicable)
│   └── App.*            # App entry point
├── package.json / csproj / etc
└── README.md
```

## ⚙️ Getting Started

Follow these steps to run the project locally.

### 1. Clone the Repository

```bash
git clone https://github.com/yosephhasson/firebaseAuth.git
cd firebaseAuth
npm install
```

### 2. Install Dependencies
```bash
npm install
```

### 3. Create a Firebase Project
```text
Go to https://console.firebase.google.com/
Click Add Project
Follow the setup steps
After creation, click Web App (</>) to register your app
Copy your Firebase config values
```

### 4. Enable Authentication
```text
In Firebase Console, go to Authentication
Click Sign-in method
Enable:
Email/Password
Optional providers like Google or Apple
```

### 5. Configure Environment Variables
```text
Create a .env file in the root of the project:
REACT_APP_FIREBASE_API_KEY=your_api_key
REACT_APP_FIREBASE_AUTH_DOMAIN=your_project.firebaseapp.com
REACT_APP_FIREBASE_PROJECT_ID=your_project_id
REACT_APP_FIREBASE_APP_ID=your_app_id
```

### 6. Initialize Firebase
```text
Update your Firebase configuration file:
```

```typescript
const firebaseConfig = {
  apiKey: process.env.REACT_APP_FIREBASE_API_KEY,
  authDomain: process.env.REACT_APP_FIREBASE_AUTH_DOMAIN,
  projectId: process.env.REACT_APP_FIREBASE_PROJECT_ID,
  appId: process.env.REACT_APP_FIREBASE_APP_ID,
};
```

### 7. Run the Application
```bash
npm start
```

### 8. Test the App
```text
Register a new user
Log in with your credentials
Verify session persistence
Log out
```
