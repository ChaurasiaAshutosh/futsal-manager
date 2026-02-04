# ⚽ Futsal Manager App

A cross-platform Flutter application to manage futsal players, track balances, record weekly games, and redirect payments to eSewa.

This project is built **step by step** with a strong focus on:
- Clean architecture
- Git best practices
- Learning-by-building
- Future extensibility

---

## 🎯 Project Goal

This app is designed for small futsal groups where:
- Players deposit money **outside the app** (e.g., via eSewa QR)
- The app acts as a **ledger**, not a wallet
- Weekly futsal costs are split among players who played
- Payments to futsal are made manually via eSewa (app redirect only)

The app **does NOT**:
- Auto-sync with eSewa
- Handle real money
- Store sensitive payment data

---

## 🧠 Core Concepts

- **Ledger-based balance tracking**
- **Manual deposit entry**
- **Automatic weekly deduction**
- **Simple & transparent accounting**
- **No over-engineering**

> eSewa = Payment tool  
> This App = Accounting system

---

## 🧱 Tech Stack

### Frontend
- **Flutter** (single codebase)
- Target platforms:
  - Android (primary)
  - macOS (later)
  - iOS (future)

### Backend (later phase)
- **Firebase Firestore** (database)
- **Firebase Storage** (optional)

### Payments
- **eSewa deep-link redirect only**
- No SDK, no API verification

---

## 🌿 Git Branch Strategy

This repository follows a **professional Git workflow**:

