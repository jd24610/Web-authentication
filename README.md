# 🔐 SecureAuth - Premium Web Authentication 

A high-performance, professional-grade authentication system built with **Google Firebase (v10)**. This project demonstrates modern security best practices, multi-factor authentication, and a stunning Glassmorphism UI.

![Project Preview](https://img.shields.io/badge/Status-Complete-success)
![Firebase](https://img.shields.io/badge/Database-Firestore-deepskyblue)
![UI](https://img.shields.io/badge/UI-Glassmorphism-blueviolet)

---

## 🚀 Key Features

*   **🌓 Adaptive Theme Engine:** Seamless **Dark/Light Mode** switching with persistence via `localStorage`.
*   **👤 Dynamic Identity:** Automated **Avatar Generation** using user initials and stylish gradients.
*   **🛡️ Verification Gate:** Enforced **Email Verification** logic that protects the dashboard from unverified accounts.
*   **⌨️ Productivity Shortcuts:** Universal **Enter key support** for faster navigation and form submission.
*   **✨ Premium Design:** Fully responsive, glassmorphism UI with **animated background orbs**.
*   **🔒 Multi-Factor Authentication (MFA):** Professional 6-digit OTP flow with smart focus and backspace support.
*   **📱 Phone (SMS) Sign-In:** Integrated Firebase Phone Auth with invisible reCAPTCHA.
*   **🌐 Google Social Login:** One-click OAuth with automatic profile synchronization.
*   **🛠️ Advanced Signup:** Full Name capture, password strength validation, and confirmation matching.
*   **⏳ UX Polish:** Real-time Loading Spinners and smooth screen transitions.
*   **🔄 Session Persistence:** Intelligent session detection and auto-redirect.
*   **💾 Cloud Firestore:** Persistent profile storage (Names, Bios, Join Dates).
---

## 🛠️ Tech Stack

- **Frontend:** Vanilla HTML5, CSS3 (Modern Flexbox/Grid), JavaScript (ES6 Modules)
- **Backend-as-a-Service:** Google Firebase (Auth, Firestore, Analytics)
- **Styling:** Custom CSS with Glassmorphic design tokens
- **Font:** Inter (via Google Fonts)

---

## 🚦 Getting Started

### 1. Clone the repository
```bash
git clone https://github.com/your-username/web-authentication.git
```

### 2. Configure Firebase
- Create a project at [Firebase Console](https://console.firebase.google.com/).
- Enable **Email/Password**, **Google**, and **Phone** authentication.
- Create a **Cloud Firestore** database.
- Replace the `firebaseConfig` object in `index.html` with your own keys.

### 3. Run locally
You can use any local server. For example, using Python:
```bash
python3 -m http.server 8080
```
Visit `http://localhost:8080` in your browser.

---

## 🛡️ Security Implementation Details
This project focuses on the **Frontend-to-Backend** security flow:
- **Lockout Mechanism:** Utilizes `localStorage` to track failed attempts and timestamp blocks.
- **Validation:** Uses Regex for real-time password feedback.
- **Cloud Database:** Rules-based storage in Firestore to ensure each user only accesses their own profile data (`auth.currentUser.uid`).

---

## 📄 License
This project is open-source and available under the [MIT License](LICENSE).
