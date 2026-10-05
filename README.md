<div align="center">

# 🃏 Scrum Poker — Backend

**Real-time planning poker API for agile teams.**
Built with NestJS, ESM, and TypeScript.

![Node](https://img.shields.io/badge/node-%3E%3D20-339933?logo=node.js&logoColor=white)
![NestJS](https://img.shields.io/badge/NestJS-E0234E?logo=nestjs&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?logo=typescript&logoColor=white)
![Vitest](https://img.shields.io/badge/tested%20with-Vitest-6E9F18?logo=vitest&logoColor=white)
![License](https://img.shields.io/badge/license-UNLICENSED-lightgrey)

</div>

---

## ✨ Overview

Scrum Poker lets distributed teams estimate stories together in real time. This repository contains the **backend API** that powers sessions, voting, and reveals.

## 🧱 Tech Stack

| Layer         | Technology                                  |
| ------------- | ------------------------------------------- |
| Framework     | [NestJS](https://nestjs.com/)               |
| Language      | TypeScript (ESM)                            |
| Testing       | Vitest (unit + e2e)                         |
| Linting       | Oxlint                                      |
| Observability | `@nestjs/observe` (tracing, logs, metrics)  |

## 📋 Requirements

- Node.js **20+**
- npm **10+**

## 🚀 Getting Started

```bash
git clone https://github.com/Gemeda4927/scrum-poker.git
cd scrum-poker
npm install
```

Create your environment file:

```cmd
copy .env.example .env
```

Then fill in the values (see [Environment](#-environment)).

## ▶️ Run

```bash
npm run start:dev     # watch mode (development)
npm run start         # standard
npm run build         # compile for production
npm run start:prod    # run compiled build
```

Server runs at **http://localhost:3000**

## 🧪 Test

```bash
npm run test          # unit tests
npm run test:e2e      # end-to-end tests
npm run test:cov      # coverage report
```

## 🧹 Lint & Format

```bash
npm run lint
npm run format
```

## 📜 Scripts

| Script              | What it does                    |
| ------------------- | ------------------------------- |
| `npm run start:dev` | Start in watch mode             |
| `npm run start`     | Start the app                   |
| `npm run build`     | Compile TypeScript              |
| `npm run start:prod`| Run the production build        |
| `npm run test`      | Run unit tests                  |
| `npm run test:e2e`  | Run end-to-end tests            |
| `npm run test:cov`  | Run tests with coverage         |
| `npm run lint`      | Lint with Oxlint                |
| `npm run format`    | Format the codebase             |

## 📁 Project Structure

```text
scrum-poker/
├── src/
│   ├── main.ts             # entry point
│   ├── app.module.ts       # root module
│   ├── app.controller.ts   # root controller
│   └── app.service.ts      # root service
├── test/                   # e2e tests
├── .env.example            # environment template
└── README.md
```

## 🔐 Environment

| Variable             | Description                      | Default       |
| -------------------- | -------------------------------- | ------------- |
| `PORT`               | Server port                      | `3000`        |
| `NODE_ENV`           | `development` or `production`    | `development` |
| `OBSERVE_APP_KEY`    | `@nestjs/observe` app key        | —             |
| `OBSERVE_APP_SECRET` | `@nestjs/observe` app secret     | —             |

> ⚠️ Never commit your `.env` file.

## ⚠️ ESM Note

This project uses ES Modules. Relative imports **must include the `.js` extension**:

```ts
import { AppService } from './app.service.js';
```

## 🗺️ Roadmap

- [ ] Session (room) creation and joining
- [ ] Real-time voting via WebSockets
- [ ] Reveal and reset rounds
- [ ] Story queue and estimate history
- [ ] Authentication
- [ ] Docker setup and CI pipeline

## 🤝 Contributing

1. Fork the repo
2. Create a branch: `git checkout -b feature/my-feature`
3. Commit your changes: `git commit -m "feat: add my feature"`
4. Push: `git push origin feature/my-feature`
5. Open a Pull Request

## 📄 License

**UNLICENSED** — private project.

---

<div align="center">

Built by [Gemeda Tamiru](https://github.com/Gemeda4927)

</div>