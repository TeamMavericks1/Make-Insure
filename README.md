# 🛡️ Make Insure (Full-Stack Super App)

**Next-Generation Insurance Claim Verification & User Portal**

Make Insure is a comprehensive, full-stack insurance application built to solve the dual-sided failure of modern insurance systems: catching fraudulent claims *before* payout while providing a seamless, personalized dashboard experience for legitimate users.

---

## 🚀 The Vision
Moving beyond a simple verification tool, Make Insure offers a complete user ecosystem. It integrates a real-time AI-driven fraud gatekeeper with a modern user dashboard, curated policy offers, and persistent claim tracking, proving that enterprise-grade security can coexist with beautiful UI/UX.

## ✨ Key Features

* **Real-Time AI Auditor:** The core engine. It intercepts claims at submission, applying dynamic financial ratio checks to instantly triage claims into Auto-Approved, Manual Review, or Total Fraud.
* **Dynamic Dashboard:** A central hub that reads from persistent browser storage to display real-time statistics on total claims audited, fraud prevented, and pending reviews.
* **Interactive Policy Offers:** An animated, responsive marketplace featuring curated insurance packages across Health, Vehicle, Tech, and Travel domains.
* **Profile & Settings Vault:** A state-driven user profile page featuring interactive, expandable panels for Security Settings, UPI Payment Management, and an Insurance Document Vault.
* **Persistent Audit Ledger:** A live history table that securely logs all AI decisions, timestamps, and risk scores using `localStorage` so data survives page refreshes.

---

## 🛠️ Tech Stack & Architecture

### Frontend (The User Portal)
* **React.js** (Bootstrapped with Vite)
* **React Router DOM** (Client-side routing for seamless, non-reloading page transitions)
* **Axios** (Asynchronous API communication)
* **State Management:** React `useState` & `useEffect` hooks coupled with HTML5 LocalStorage.

### Backend (The AI Engine)
* **Node.js & Express.js** (RESTful API architecture)
* **Multer** (Middleware for handling secure multipart/form-data image uploads)
* **CORS** (Cross-Origin Resource Sharing)

---

## 📁 Project Structure

```text
Make Insure App/
├── backend/
│   ├── uploads/            # Temporary visual evidence storage
│   ├── package.json
│   └── server.js           # Core AI logic & API endpoint
└── frontend/
    ├── src/
    │   ├── views/
    │   │   ├── Auditor/    # Form & AI Results UI
    │   │   ├── Dashboard/  # Dynamic stats & welcome screen
    │   │   ├── Offers/     # Expandable interactive policy cards
    │   │   └── Profile/    # Inline settings & vault UI
    │   ├── App.jsx         # Main Router & Navigation Switchboard
    │   └── main.jsx
    └── package.json
