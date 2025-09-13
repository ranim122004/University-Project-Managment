# UniFlow — Project Management Website (React + Firebase)

A modern web app that helps university students **track projects, plan tasks on a calendar, collaborate, and manage accounts**. Built with **React** and backed by **Firebase Authentication, Firestore, and Storage**.

## ✨ Core Features

- **Auth & Onboarding** — Email/password plus **Google, Facebook, and Twitter** sign-in options; validated sign-up/sign-in popups.
- **Dashboard** — After login, see urgent tasks (due in 3 days) and quick links to your most urgent projects. 
- **Task Calendar** — View tasks on a schedule and **jump directly to dates**. :contentReference.
- **Projects** — Create, filter (completed/uncompleted), and view all projects; open **Project Details** to edit/delete if you’re the creator.
- **Account Settings** — Update profile, change details, and **delete account** with confirmation.


## 🧠 React Architecture

- **Components & JSX** for clean, reusable UI (e.g., landing, auth popups, navbar). 
- **State Management** with `useState` for users, projects, calendar dates; custom `useSessionStorage` keeps key values across reloads. 
- **Hooks** — `useEffect` for data fetching and controlled re-renders; `useState` for component state.
  - React docs: **useEffect** and **useState**. 
- **Context API** — global auth/user context so components don’t need deep prop drilling.  
  - React docs: **Context / useContext / createContext**. 


## ☁️ Firebase Integration

- **Authentication** — email/password + federated providers (Google, Facebook, Twitter).
  - Firebase Auth overview & web start guides.
- **Firestore (NoSQL)** — documents & collections for accounts, projects, tasks; references used instead of foreign keys. 
  - Firestore data model (NoSQL, documents & collections). 
- **Storage** — profile and project images.

## 🚀 Deployment & Performance

- **Hosting** options include **Firebase Hosting** (global CDN, tight integration with Firebase services).
- **Optimization** — Componentization, updating only affected subtrees; hooks with dependencies reduce unnecessary re-renders.

## 🛠️ Getting Started

```bash
# 1) Install
npm install

# 2) Dev server
# Use the script defined in package.json:
npm start        # (Create React App)  OR
npm run dev      # (Vite)

# 3) Environment (Firebase)
# Create .env with your Firebase config, e.g.:
# VITE_API_KEY=...
# VITE_AUTH_DOMAIN=...
# VITE_PROJECT_ID=...
# VITE_STORAGE_BUCKET=...
# VITE_MESSAGING_SENDER_ID=...
# VITE_APP_ID=...
