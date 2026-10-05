markdown
# Scrum Poker — Backend

Real-time Scrum Poker API built with [NestJS](https://nestjs.com/) (ESM) and TypeScript.

## Stack

- **NestJS** — application framework
- **ESM** — ES Modules
- **Vitest** — unit & e2e testing
- **Oxlint** — fast linting
- **@nestjs/observe** — tracing, logs, metrics

## Requirements

- Node.js 20+
- npm 10+

## Setup

```bash
git clone https://github.com/Gemeda4927/scrum-poker.git
cd scrum-poker
npm install
Run
bash
npm run start:dev     # watch mode (development)
npm run start         # standard
npm run start:prod    # production (requires npm run build first)
Server runs at http://localhost:3000

Test
bash
npm run test          # unit tests
npm run test:e2e      # end-to-end tests
npm run test:cov      # coverage
Lint & Format
bash
npm run lint
npm run format
Project Structure
text
src/
├── main.ts           # entry point
├── app.module.ts     # root module
├── app.controller.ts
└── app.service.ts
test/                 # e2e tests
Environment
Copy .env.example to .env and fill in values:

bash
cp .env.example .env
Variable	Description
PORT	Server port (default 3000)
NODE_ENV	development / production
OBSERVE_APP_KEY	@nestjs/observe app key
OBSERVE_APP_SECRET	@nestjs/observe secret
Notes
This project uses ESM. Relative imports require the .js extension:

ts
import { AppService } from './app.service.js';
License
UNLICENSED — private project.

text

---

### Save it

Overwrite your current `README.md`:

```bash
cd C:\Users\HP\OneDrive\Desktop\Poker\Backend
notepad README.md
Paste, save, then:

`"# scrum-poker" 
