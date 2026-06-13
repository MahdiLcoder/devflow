<div align="center">
  <br />
  <a href="https://devflow-rose.vercel.app/" target="_blank">
    <img src="https://github.com/user-attachments/assets/769882e6-bae6-4932-a117-829cf34f809f" alt="Project Banner">
  </a>
  <br />
  <br />

  <div>
    <img src="https://img.shields.io/badge/-TypeScript-black?style=for-the-badge&logoColor=white&logo=typescript&color=3178C6" alt="typescript" />
    <img src="https://img.shields.io/badge/-Next_JS-black?style=for-the-badge&logoColor=white&logo=nextdotjs&color=000000" alt="nextdotjs" />
    <img src="https://img.shields.io/badge/-Tailwind_CSS-black?style=for-the-badge&logoColor=white&logo=tailwindcss&color=06B6D4" alt="tailwindcss" />
    <img src="https://img.shields.io/badge/-MongoDB-black?style=for-the-badge&logoColor=white&logo=mongodb&color=47A248" alt="mongodb" />
    <img src="https://img.shields.io/badge/-ShadCN_UI-black?style=for-the-badge&logoColor=white&logo=shadcnui&color=000000" alt="shadcnui" />
    <img src="https://img.shields.io/badge/-Open_AI-black?style=for-the-badge&logoColor=white&logo=openai&color=412991" alt="openai" />
  </div>
</div>

# DevFlow 💻🚀

🔗 **Live Demo**: [devflow-rose.vercel.app](https://devflow-rose.vercel.app/)

DevFlow is a modern, full-stack community-driven platform inspired by StackOverflow. It serves as a space for developers to ask questions, share knowledge, collaborate, and grow together. The platform features advanced capabilities including AI-powered answers, a global recommendation system, voting/reputation dynamics, gamified badges, and a custom job search module.

Developed using Next.js 15, React, TypeScript, TailwindCSS, MongoDB, and NextAuth.js.

---

## 🚀 Key Features

*   **Authentication**: Secure authentication supporting OAuth (GitHub, Google) and email/password credentials.
*   **Global Search & Filter**: Instant, site-wide search across questions, users, tags, and answers with robust filtering and pagination.
*   **AI-Generated Answers**: Integrated OpenAI API to generate smart, contextual answers to questions on demand.
*   **Reputation & Gamification**: User reputation points tracking system with automated badge assignments (Bronze, Silver, Gold) based on community contributions.
*   **Rich MDX Editor**: Dynamic text editor supporting code syntax highlighting, rich text, and preview mode for asking questions and writing answers.
*   **Voting System**: Interactive upvoting and downvoting on questions and answers to bubble up high-quality content.
*   **Collections & Bookmarks**: Save favorite questions to a personal collection space for quick future reference.
*   **Job Finder**: Built-in job search module integrated with external job APIs, allowing filtering by location and role.
*   **Responsive Theme System**: Full light/dark mode support with sleek, responsive designs optimized for mobile, tablet, and desktop views.

---

## 🛠️ Tech Stack

*   **Framework**: [Next.js](https://nextjs.org/) (App Router, Server Components & Server Actions)
*   **Styling**: [TailwindCSS](https://tailwindcss.com/), [ShadCN UI](https://ui.shadcn.com/)
*   **Language**: [TypeScript](https://www.typescriptlang.org/)
*   **Database**: [MongoDB](https://www.mongodb.com/) (using Mongoose for schemas & models)
*   **Authentication**: [NextAuth.js](https://next-auth.js.org/) (Auth.js v5)
*   **AI Integration**: [OpenAI API](https://openai.com/)
*   **Form Management**: [React Hook Form](https://react-hook-form.com/), [Zod](https://zod.dev/)
*   **Editor**: [TinyMCE WYSIWYG Editor](https://www.tiny.cloud/)

---

## ⚙️ Quick Start

Follow these steps to set up and run the project locally on your machine.

### Prerequisites

Make sure you have the following installed:
*   [Node.js](https://nodejs.org/) (v18+ recommended)
*   [MongoDB](https://www.mongodb.com/try/download/community) (Local instance or Atlas connection URI)
*   [Git](https://git-scm.com/)

### 1. Clone the Repository

```bash
git clone https://github.com/MahdiLcoder/devflow.git
cd devflow
```

### 2. Install Dependencies

```bash
npm install
```

### 3. Set Up Environment Variables

Create a `.env.local` file in the root of the project and supply the following variables:

```env
# Database Configuration
MONGODB_URI=your_mongodb_connection_string

# OpenAI API Key for AI Answers
OPENAI_API_KEY=your_openai_api_key

# RapidAPI Key (for Job Search functionality)
NEXT_PUBLIC_RAPID_API_KEY=your_rapidapi_key

# Auth configuration
AUTH_SECRET=your_auth_secret_key # run `npx auth secret` to generate
NEXTAUTH_URL=http://localhost:3000

# Google OAuth Credentials
AUTH_GOOGLE_ID=your_google_client_id
AUTH_GOOGLE_SECRET=your_google_client_secret

# GitHub OAuth Credentials
AUTH_GITHUB_ID=your_github_client_id
AUTH_GITHUB_SECRET=your_github_client_secret

# TinyMCE Editor Key
NEXT_PUBLIC_TINY_EDITOR_API_KEY=your_tinymce_api_key

# Server & App URL
NEXT_PUBLIC_SERVER_URL=http://localhost:3000
```

### 4. Run the Development Server

```bash
npm run dev
```

Open [http://localhost:3000](http://localhost:3000) in your browser to view the application in action.

---

## 📂 Project Structure

```text
├── app/                  # Next.js App Router (pages, APIs, layouts)
├── components/           # Reusable UI components (shared & feature-specific)
│   └── ui/               # ShadCN UI primitive components
├── constants/            # Site configurations, menus, and static lists
├── context/              # React Context providers (theme, auth state)
├── database/             # MongoDB schema models & database connection utilities
├── hooks/                # Custom React hooks
├── lib/                  # Helper utilities, actions, and validation schemas (Zod)
├── public/               # Static assets (images, icons, vectors)
└── types/                # TypeScript interfaces and type definitions
```
