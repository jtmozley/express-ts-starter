# express-ts-starter

A minimal, production-ready starter template for building **Express.js APIs** using **TypeScript** and **Bun**. Includes common middleware, linting, formatting, and environment configuration out of the box to help you scaffold quickly, stay consistent, and ship with confidence.

[![Deploy on Railway](https://railway.com/button.svg)](https://railway.com/deploy/express-ts-starter?referralCode=WTgsfh&utm_medium=integration&utm_source=template&utm_campaign=generic)

---

## Features

- Express.js server with TypeScript for type safety
- Bun runtime and lockfile for fast installs and startup
- Project structure ready for routing, middleware, and scaling
- Compression, JSON parsing, security headers, and request logging
- `/misc/status` health endpoint for deployment checks
- ESLint and Prettier for linting and formatting
- `.env.template` for environment variable setup

---

## Getting Started

### Prerequisites

- **Bun 1.3.14**
- Optional: A code editor with TypeScript and linting support

### Setup

```bash
# Clone the repo
git clone https://github.com/jtmozley/express-ts-starter.git
cd express-ts-starter

# Install dependencies
bun install
```

### Environment Variables

Rename the .env.template file and fill in required values:

```bash
mv .env.template .env
```

### Development

```bash
bun run dev
```

### Run (Production)

```bash
bun run start
```

### Status Check

```text
GET /misc/status
```

```json
{
  "status": "online"
}
```

### Project Structure

```text
express-ts-starter/
├── .env.template         # Environment variable template
├── .eslintrc.json        # ESLint configuration
├── .prettierrc.json      # Prettier formatting rules
├── .gitignore
├── bun.lock              # Bun lockfile
├── package.json
├── tsconfig.json
└── src/
    ├── express.config.ts   # Middleware and route configurations 
    ├── server.ts           # Entry point of the application
    ├── routes/             # API route handlers
    └── (other folders as needed for controllers, middleware, etc.)
```
