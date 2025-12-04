# BeatCode - LeetCode Questions Tracker

BeatCode is a sophisticated, full-stack web application designed for tracking and managing coding interview questions. Built with a modern tech stack, it provides a comprehensive platform for users to manage LeetCode-style questions with advanced progress tracking, analytics, and administrative capabilities.


## 📋 Table of Contents

- [About The Project](#-about-the-project)
- [Key Features](#-key-features)
- [Tech Stack](#-tech-stack)


---

## 🎯 About The Project

This application serves as a personal coding question tracker to help users prepare for technical interviews. It allows users to manage a large list of questions, track their progress (Solved, Attempted, Favorited), add personal notes, and visualize their performance through an analytics dashboard. It includes a multi-tiered role system (User, Admin, Super Admin) and provides limited access for guest users to explore the platform.

---

## ✨ Key Features

-   **👤 User Authentication**: Secure sign-up and login system using NextAuth.js with role-based access control.
-   **📊 Comprehensive Question Management**: Full CRUD operations for questions, including bulk CSV import for administrators.
-   **📈 Advanced Progress Tracking**: Users can mark questions as solved, attempted, or favorited, and add personal remarks.
-   **⚙️ Powerful Filtering & Search**: Filter questions by difficulty, company, topics, and status, with a debounced real-time search.
-   **📈 Analytics Dashboard**: Interactive charts and statistics to visualize user progress by difficulty, company, topic, and over time.
-   **👑 Admin Panel**: Manage users, import/export questions, and view system-wide statistics.
-   **👻 Guest Access**: Guests can browse a limited set of 500 questions to preview the platform's features.

---

## 🛠 Tech Stack

-   **Framework**: Next.js 14 (App Router)
-   **Language**: TypeScript
-   **Database**: PostgreSQL
-   **ORM**: Prisma
-   **Authentication**: NextAuth.js
-   **Styling**: Tailwind CSS
-   **UI Components**: Shadcn/ui, Radix UI
-   **State Management**: Zustand
-   **Form Handling**: React Hook Form
-   **Data Visualization**: Chart.js

---



# Development Configuration
NODE_ENV="development"
