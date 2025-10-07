# BeatCode - LeetCode Questions Tracker

BeatCode is a sophisticated, full-stack web application designed for tracking and managing coding interview questions. Built with a modern tech stack, it provides a comprehensive platform for users to manage LeetCode-style questions with advanced progress tracking, analytics, and administrative capabilities.


## 📋 Table of Contents

- [About The Project](#-about-the-project)
- [Key Features](#-key-features)
- [Tech Stack](#-tech-stack)
- [Getting Started](#-getting-started)
- [Environment Variables](#-environment-variables)
- [Usage](#-usage)
- [Future Improvements](#-future-improvements)

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

## 🚀 Getting Started

Follow these instructions to get a copy of the project up and running on your local machine.

### Prerequisites

-   Node.js (v18.0 or higher)
-   PostgreSQL (v12 or higher)
-   npm or yarn

### Installation

1.  **Clone the repository**
    ```bash
    git clone <repository-url>
    cd BeatCode
    ```

2.  **Install dependencies**
    ```bash
    npm install
    # or
    yarn install
    ```

3.  **Set up environment variables**
    -   Copy the `.env.example` file to a new file named `.env`.
    -   Update the `.env` file with your database URL and other credentials. See the section below for details.

4.  **Set up the database**
    -   This single command will generate the Prisma client, push the schema to your database, and seed it with initial data and admin users.
    ```bash
    npm run db:setup
    ```

5.  **Run the development server**
    ```bash
    npm run dev
    ```
    The application will be available at `http://localhost:3000`.

---

## ⚙️ Environment Variables

Create a `.env` file in the root directory and add the following variables:

```env
# Database Configuration
DATABASE_URL="postgresql://USERNAME:PASSWORD@HOST:PORT/DATABASE?schema=public"

# NextAuth.js Configuration
NEXTAUTH_SECRET="your-super-secret-key"
NEXTAUTH_URL="http://localhost:3000"

# Admin User Configuration (used for seeding)
SUPER_ADMIN_EMAIL="superadmin@example.com"
SUPER_ADMIN_PASSWORD="YourSecurePassword123"
SUPER_ADMIN_NAME="Super Admin"
SUPER_ADMIN_USERNAME="superadmin"

ADMIN_EMAIL="admin@example.com"
ADMIN_PASSWORD="YourSecurePassword123"
ADMIN_NAME="Admin User"
ADMIN_USERNAME="admin"

# Development Configuration
NODE_ENV="development"
