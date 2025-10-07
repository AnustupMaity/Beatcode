# BeatCode - LeetCode Questions Tracker

A full-stack web application for tracking and managing coding interview questions, built with Next.js 14, TypeScript, PostgreSQL, and modern web technologies.

## 📋 Table of Contents
- [Overview](#overview)
- [Features](#features)
- [Tech Stack](#tech-stack)
- [Installation & Setup](#installation--setup)
- [Usage](#usage)
- [Contributing](#contributing)

## 🎯 Overview

BeatCode is a question tracking system designed for coding interview preparation. Track your progress on LeetCode-style questions with analytics and administrative capabilities.

### Key Features
- **Question Management**: Browse, filter, and search through coding problems
- **Progress Tracking**: Mark questions as solved, attempted, or favorited
- **User Roles**: Support for Users, Admins, and Super Admins
- **Guest Access**: Browse up to 500 questions without registration
- **Analytics Dashboard**: Visualize your progress with charts and statistics
- **CSV Import**: Bulk import questions (Admin feature)

## ✨ Features

### For Users
- **Question Browser**: Filter by difficulty, company, topics, and timeline
- **Progress Tracking**: Track solved, attempted, and favorited questions
- **Personal Notes**: Add remarks and insights to questions
- **Analytics Dashboard**: View progress statistics with interactive charts
- **Search**: Real-time search across all questions

### For Admins
- **User Management**: View and manage all registered users
- **CSV Import**: Bulk import questions from CSV files
- **Question CRUD**: Create, update, and delete questions
- **System Statistics**: Monitor platform usage and activity

### For Guests
- **Limited Browsing**: Access up to 500 questions without registration
- **Basic Filtering**: Search and filter available questions

## 🛠 Tech Stack

### Frontend
- **Next.js 14** - React framework with App Router
- **TypeScript** - Type-safe development
- **Tailwind CSS** - Utility-first styling
- **Shadcn/ui** - UI component library
- **Chart.js** - Data visualization
- **Zustand** - State management

### Backend
- **Next.js API Routes** - RESTful API endpoints
- **Prisma ORM** - Database management
- **PostgreSQL** - Primary database
- **NextAuth.js** - Authentication
- **Bcrypt** - Password hashing

### Development Tools
- **ESLint** - Code linting
- **Prettier** - Code formatting
- **TypeScript** - Static type checking



## 🚀 Installation & Setup

### Prerequisites
- Node.js v18.0 or higher
- PostgreSQL v12 or higher
- npm or yarn package manager

### Installation Steps

1. **Clone the repository**
```bash
git clone <repository-url>
cd Beatcode
```

2. **Install dependencies**
```bash
npm install
```

3. **Set up environment variables**
Create a `.env` file in the root directory:
```env
DATABASE_URL="postgresql://postgres:password@localhost:5432/beatcode"
NEXTAUTH_SECRET="your-secret-key"
NEXTAUTH_URL="http://localhost:3000"

SUPER_ADMIN_EMAIL="admin@beatcode.com"
SUPER_ADMIN_PASSWORD="Admin@123"
```

4. **Set up the database**
```bash
npm run db:setup
```

5. **Start the development server**
```bash
npm run dev
```

Visit `http://localhost:3000` to access the application.

## 📖 Usage

### Getting Started
1. **Sign up** for an account or browse as a guest
2. **Filter questions** by difficulty, company, or topic
3. **Mark progress** as you solve problems
4. **Track statistics** in your analytics dashboard

### Admin Features
- **Import questions** from CSV files (max 5MB)
- **Manage users** and assign roles
- **View system statistics** and monitor activity

### Tips
- Use filters to find relevant questions
- Add personal notes to questions for future reference
- Check your progress dashboard regularly
- Guest users can browse up to 500 questions

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

### Development
1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📝 License

This project is open source and available under the MIT License.

## 📧 Contact

For questions or support, please open an issue on GitHub.

---

Made with ❤️ for coding interview preparation