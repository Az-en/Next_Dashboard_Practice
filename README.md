# Next.js Full-Stack Dashboard

A modern, high-performance web dashboard built with **Next.js 14**, **React**, **TypeScript**, and **Tailwind CSS**.

This project was built to master the Next.js App Router paradigm. It bridges the gap between complex server-side logic and clean, responsive user interfaces, demonstrating a complete full-stack workflow from database querying to secure authentication.

---

## 🚀 Test Credentials
To explore the dashboard's authenticated features, please use the following test account:
- **Email:** `user@nextmail.com`
- **Password:** `123456`

---

## 🧠 Key Learning Outcomes & Implementations

This project goes beyond basic UI components, implementing production-ready Next.js features:

### 1. Modern Architecture & Routing
- **App Router:** Utilized the new App Router (`app/` directory) for intuitive, file-system-based routing.
- **Layouts & Pages:** Implemented shared layouts that persist state across navigation, preventing expensive re-renders.
- **Dynamic Routing:** Handled dynamic segments for individual data views and modification pages.

### 2. Advanced Data Fetching & State
- **React Server Components (RSC):** Shifted data fetching to the server to reduce the client-side JavaScript bundle and securely access backend resources.
- **Streaming & Suspense:** Implemented React Suspense boundaries to stream UI components as data becomes available, significantly improving perceived load times and avoiding waterfall requests.
- **URL-Based State:** Managed search filters and pagination directly through URL search parameters, allowing users to share and bookmark specific dashboard states.

### 3. Server-Side Mutations
- **Server Actions:** Replaced traditional API endpoints with Server Actions for handling form submissions (Create, Update, Delete) directly on the server, ensuring type safety and seamless revalidation.
- **Cache Revalidation:** Utilized `revalidatePath` to instantly update the UI after database mutations without requiring a full page reload.

### 4. Security & Authentication
- **NextAuth.js:** Implemented a robust credentials-based authentication flow.
- **Middleware:** Utilized Next.js Middleware to protect private routes, seamlessly redirecting unauthenticated users to the login screen.
- **Password Hashing:** Secured user data using `bcrypt` for password hashing and validation.

### 5. Error Handling & Accessibility
- **Graceful Error States:** Implemented custom `error.tsx` and `not-found.tsx` boundaries to catch runtime errors and missing resources without breaking the app.
- **Form Validation:** Used **Zod** for strict schema validation on the server before mutating the database.
- **Optimized UI:** Leveraged `next/font` and `next/image` to prevent layout shifts and optimize core web vitals.

---

## 🛠️ Tech Stack

- **Framework:** Next.js (App Router)
- **Library:** React.js
- **Language:** TypeScript
- **Styling:** Tailwind CSS
- **Database:** Supabase (Vercel Postgres)
- **Authentication:** NextAuth.js
- **Validation:** Zod

---

## 💻 Local Development

To run this project locally, follow these steps:

**1. Clone the repository:**
```bash
git clone [https://github.com/Az-en/Next_Practice.git](https://github.com/Az-en/Next_Practice.git)
cd Next_Practice