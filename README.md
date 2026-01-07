# 🧠 PixelMind — AI Image Generation Platform

**PixelMind** is a modern AI-powered image generation platform that enables users to create stunning visuals and train custom AI models using their own image datasets. Designed for creators, developers, and AI enthusiasts, PixelMind combines a sleek interface with a powerful backend to deliver high-quality, personalized AI-generated images.

Whether you're building AI-driven products or exploring creative workflows, PixelMind gives you the tools to turn ideas into visuals.

---

## ✨ Features

* AI-powered image generation
* Custom model training with user datasets
* Secure authentication & authorization
* Image gallery with preview & download
* Fully responsive modern UI
* Scalable monorepo architecture

---

## 🧰 Tech Stack

* **Frontend**: Next.js 14 (App Router), TypeScript, Tailwind CSS, Shadcn/UI
* **Backend**: Node.js with TypeScript
* **Authentication**: Clerk
* **Monorepo**: Turborepo
* **Package Manager**: Bun
* **Containerization**: Docker

---

## 📁 Project Structure

### Apps & Packages

* `apps/web` – Next.js frontend
* `apps/backend` – Node.js backend service
* `packages/ui` – Shared React UI components
* `packages/typescript-config` – Shared TypeScript configuration
* `packages/eslint-config` – Shared ESLint configuration

```
.
├── apps
│   ├── web/                 # Next.js frontend
│   └── backend/             # Node.js backend
├── packages
│   ├── ui/                  # Shared UI components
│   ├── typescript-config/   # Shared TS config
│   └── eslint-config/       # Shared ESLint config
├── docker/                  # Docker configuration
│   ├── Dockerfile.frontend
│   └── Dockerfile.backend
└── package.json
```

---

## 🚀 Getting Started

### Prerequisites

* Docker
* Bun
* Clerk account (for authentication)

---

### 🔐 Environment Setup

Create the following environment files:

```bash
# apps/web/.env.local
NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY=your_publishable_key
CLERK_SECRET_KEY=your_secret_key
NEXT_PUBLIC_BACKEND_URL=http://localhost:8080
```

---

### 💻 Local Development

```bash
# Install dependencies
bun install

# Run all apps in development mode
bun run dev

# Build all packages
bun run build
```

---

## 🧪 Development Commands

```bash
# Run frontend only
bun run start:web

# Run backend only
bun run start:backend

# Run both frontend and backend
bun run dev
```

---

## 🐳 Docker Setup

### Required Environment Variables

```bash
# Frontend
NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY=your_publishable_key
NEXT_PUBLIC_BACKEND_URL=https://api.pixelmind.yourdomain.com
NEXT_PUBLIC_STRIPE_KEY=your_stripe_key
CLERK_SECRET_KEY=your_clerk_secret_key

# Backend
DATABASE_URL=your_database_url
```

---

### Docker Commands

```bash
# Navigate to docker directory
cd docker

# Build Docker images
docker build -f Dockerfile.frontend -t pixelmind-frontend ..
docker build -f Dockerfile.backend -t pixelmind-backend ..

# Run frontend
docker run -p 3000:3000 pixelmind-frontend

# Run backend
docker run -p 8080:8080 pixelmind-backend
```

---

## 🤝 Contributing

Contributions are welcome!

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/new-feature`)
3. Commit your changes (`git commit -m "Add new feature"`)
4. Push to the branch (`git push origin feature/new-feature`)
5. Open a Pull Request

---

## 📄 License

This project is licensed under the **MIT License**.
See the `LICENSE` file for more details.

---

If you like it please give a ⭐️

