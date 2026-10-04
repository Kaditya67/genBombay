# genBombay

A full-stack modern web application built using **Next.js 15 (App Router)**, **TypeScript**, **Tailwind CSS v4**, and **Prisma ORM** with **PostgreSQL**.

---

## 🚀 Features

- **Next.js 15 App Router**: Server and client component architecture powered by Turbopack.
- **Prisma ORM & PostgreSQL**: Type-safe database schema modeling and automated queries.
- **RESTful API Routes**: Built-in backend endpoints (`/api/users`) handling CRUD operations.
- **Tailwind CSS v4 & PostCSS**: Modern styling, typography, and responsive layouts.
- **TypeScript**: Strict type-checking and end-to-end type safety across client and server.

---

## 🛠️ Tech Stack

- **Framework**: [Next.js 15](https://nextjs.org/) (App Router & Turbopack)
- **Frontend**: [React 19](https://react.dev/), [Tailwind CSS v4](https://tailwindcss.com/)
- **Backend / Database**: [Prisma ORM](https://www.prisma.io/), [PostgreSQL](https://www.postgresql.org/)
- **Language**: [TypeScript](https://www.typescriptlang.org/)

---

## 📂 Project Structure

```text
genBombay/
├── prisma/
│   └── schema.prisma         # Database models (User model & Postgres config)
├── public/                   # Static assets & SVG icons
├── src/
│   ├── app/
│   │   ├── api/
│   │   │   └── users/        # User CRUD API endpoints (GET, POST)
│   │   ├── favicon.ico
│   │   ├── globals.css       # Tailwind CSS v4 directives
│   │   ├── layout.tsx        # Root application layout
│   │   └── page.tsx          # Landing / home page
│   └── lib/
│       └── prisma.ts         # Global Prisma client singleton instance
├── .env.example              # Sample environment configuration
├── .gitignore                # Node.js, Next.js, and Prisma ignore rules
├── next.config.ts            # Next.js build configuration
├── package.json              # App scripts & dependencies
├── tsconfig.json             # TypeScript compiler settings
└── README.md
```

---

## ⚡ Getting Started

### 1. Prerequisites

- [Node.js](https://nodejs.org/) (v18.18 or higher recommended)
- [PostgreSQL](https://www.postgresql.org/) database (local instance, Supabase, Neon, or Railway)
- `npm` or `pnpm` or `yarn`

### 2. Clone the Repository

```bash
git clone https://github.com/Kaditya67/genBombay.git
cd genBombay
```

### 3. Install Dependencies

```bash
npm install
```

### 4. Configure Environment Variables

Create a `.env` file in the root directory based on [`.env.example`](.env.example):

```env
DATABASE_URL="postgresql://postgres:password@localhost:5432/genbombay?schema=public"
```

### 5. Run Database Migrations

Generate Prisma Client and push database schema:

```bash
npx prisma generate
npx prisma db push
```

### 6. Run the Development Server

```bash
npm run dev
```

Open [http://localhost:3000](http://localhost:3000) in your browser to see the result.

---

## 🌐 API Endpoints

| Method | Endpoint | Description |
| :--- | :--- | :--- |
| `GET` | `/api/users` | Fetch all users from the database |
| `POST` | `/api/users` | Create a new user (`{ "name": "...", "email": "..." }`) |

---

## 📜 License

Created for project and development purposes.

