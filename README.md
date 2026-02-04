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


### Rules
- ❌ Never develop directly on `main`
- ✅ All work happens on `dev`
- ✅ `main` is updated only after features are stable
- ✅ Every logical step = one commit

---

## 🧩 Planned Features

### Phase 1 (Core MVP)
- Player management
- Balance tracking
- Weekly game deduction
- eSewa redirect for payment
- Basic history

### Phase 2 (Enhancements)
- Game history view
- Monthly summaries
- Export to CSV
- Multiple futsal groups

### Phase 3 (Monetization)
- Freemium model
- In-app subscriptions
- Ads in free tier

---

## 🗂️ Project Structure

lib/
├── main.dart
├── app.dart
├── core/
│ ├── constants/
│ ├── utils/
│ └── theme/
├── features/
│ ├── players/
│ │ ├── player_model.dart
│ │ ├── player_service.dart
│ │ └── player_screen.dart
│ ├── games/
│ │ ├── game_model.dart
│ │ ├── game_service.dart
│ │ └── game_screen.dart
│ └── payments/
│ └── esewa_service.dart
└── services/
└── firebase_service.dart



This **feature-based architecture** allows easy addition of new features without refactoring existing code.

---

## 🧠 Development Philosophy

1. **Design first**
2. **Logic second**
3. **Persistence last**

We intentionally:
- Build logic before connecting Firebase
- Use mock/in-memory data initially
- Avoid premature optimization

This keeps the project:
- Easy to understand
- Easy to debug
- Easy to extend

---

## 🚧 Current Status

- ✅ Flutter project initialized
- ✅ Git & SSH configured
- ✅ Branch strategy in place
- ⏳ Android SDK setup in progress
- ⏳ Firebase integration pending

---

## 🛠️ How to Run (Later)

```bash
flutter pub get
flutter run

