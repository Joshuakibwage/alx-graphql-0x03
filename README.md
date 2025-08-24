# ⚡ ReactGuard: Mastering Error Handling

> **A Next.js + TypeScript project that implements robust error handling with React Error Boundaries and Sentry integration.**

---

## 📌 Project Overview

This project demonstrates how to **gracefully handle runtime errors** in a Next.js application by implementing an `ErrorBoundary` component.  
Key features include:

- A reusable `ErrorBoundary` class component in TypeScript
- Integration with **Sentry** for production-grade error monitoring
- A fallback UI with recovery options for users
- An `ErrorProneComponent` to test error handling in real scenarios

This setup ensures your app won’t crash completely when one component fails — improving **stability, reliability, and user experience**.

---

## 🎯 Learning Objectives

By completing this project, you will learn how to:

- Understand how **React Error Boundaries** work
- Implement **class components with TypeScript**
- Gracefully handle runtime errors in **Next.js**
- Integrate **third-party monitoring tools** (Sentry)
- Test error handling workflows with a controlled error-prone component

---

## 🧩 Key Concepts

- **Error Boundaries** → Special React components that catch JavaScript errors in child components  
- **Lifecycle Methods** → `getDerivedStateFromError` & `componentDidCatch` for error handling  
- **Fallback UI** → Display user-friendly error messages instead of a blank screen  
- **Error Recovery** → Add “Try Again” functionality to recover from non-critical errors  
- **Error Monitoring** → Use **Sentry** to log and track errors in production  

---

## 🛠️ Tech Stack

- **React** – UI library  
- **Next.js** – React framework for SSR and routing  
- **TypeScript** – Strongly typed JavaScript  
- **Sentry** – Error monitoring and tracking  
- **Node.js / npm** – Runtime & package management  

---

## 🌍 Real-World Use Case

Error boundaries are widely used in production apps to:  
1. Prevent full app crashes from isolated component failures  
2. Provide meaningful error messages to users  
3. Track issues with monitoring tools like **Sentry**  
4. Allow graceful recovery with retry options  
5. Maintain user trust and a seamless experience  

> Major platforms (Airbnb, Twitter, GitHub, etc.) use similar error handling patterns.

---

## 🚀 Implementation Summary

- ✅ Created `ErrorBoundary` as a **TypeScript class component**  
- ✅ Wrapped the **Next.js `_app.tsx`** with `ErrorBoundary`  
- ✅ Built an `ErrorProneComponent` to simulate runtime errors  
- ✅ Integrated **Sentry SDK** for error monitoring  
- ✅ Added fallback UI with a **retry button**  

---

## 📂 Project Structure

```bash
alx-graphql-0x03/
│
├── alx-rick-and-morty-app/
│   ├── components/
│   │   ├── ErrorBoundary.tsx       # Error Boundary implementation
│   │   ├── ErrorProneComponent.tsx # Test component that throws errors
│   │
│   ├── pages/
│   │   ├── _app.tsx                # Wrapped with ErrorBoundary
│   │   ├── index.tsx               # Example usage of ErrorProneComponent
│   │
│   ├── package.json
│   ├── README.md

⚙️ Setup & Installation

    Clone the repo

git clone https://github.com/Joshuakibwage/alx-graphql-0x03.git
cd alx-graphql-0x03/alx-rick-and-morty-app

Install dependencies

npm install

Run the development server

npm run dev

Open your browser at 👉 http://localhost:3000
🔍 Testing Error Handling

    Render the ErrorProneComponent in pages/index.tsx

    Visit the page and trigger the error

    Observe the fallback UI with the retry option

    If Sentry is configured, check the Sentry dashboard for captured errors

📡 Error Monitoring with Sentry

To enable error monitoring:

    Install Sentry:

npm install @sentry/react @sentry/nextjs

---

👨‍💻 Author

ReactGuard Project – ALX Advanced Frontend Program
Built with ❤️ to master error handling in modern React apps.
