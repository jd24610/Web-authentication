# 🔐 SecureAuth - Premium Web Authentication 

A high-performance, professional-grade authentication system built with **Google Firebase (v10)**. This project demonstrates modern security best practices, multi-factor authentication, and a stunning Glassmorphism UI.

![Project Preview](https://img.shields.io/badge/Status-Complete-success)
![Firebase](https://img.shields.io/badge/Database-Firestore-deepskyblue)
![UI](https://img.shields.io/badge/UI-Glassmorphism-blueviolet)

---

## 🚀 Key Features

*   **🔒 Multi-Factor Authentication (MFA):** Simulated 6-digit OTP verification for enhanced account security.
*   **📱 Phone (SMS) Sign-In:** Integrated Firebase Phone Authentication with invisible reCAPTCHA protection.
*   **🌐 Google Social Login:** Seamless one-click authentication using Google OAuth.
*   **🛠️ Password Security:** Real-time password strength validation rules (Length, Case, Numbers, Symbols).
*   **📉 Smart Account Lockout:** Automatic 30-second block after 3 failed login attempts to prevent brute-force attacks.
*   **💾 Cloud Profile Storage:** Persistent user data saved to **Cloud Firestore** (Display Names, Bios).
*   **📧 Password Recovery:** Integrated "Forgot Password" automated email recovery system.
*   **✨ Premium Design:** Fully responsive, dark-mode Glassmorphism UI with smooth backdrop blurs and CSS transitions.

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
