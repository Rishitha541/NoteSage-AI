# Workspace

## Overview

pnpm workspace monorepo using TypeScript. Each package manages its own dependencies.

## Stack

- **Monorepo tool**: pnpm workspaces
- **Node.js version**: 24
- **Package manager**: pnpm
- **TypeScript version**: 5.9
- **API framework**: Express 5
- **Database**: PostgreSQL + Drizzle ORM
- **Validation**: Zod (`zod/v4`), `drizzle-zod`
- **API codegen**: Orval (from OpenAPI spec)
- **Build**: esbuild (CJS bundle)
- **AI**: OpenAI via Replit AI Integrations (`gpt-5.2`)

## Artifacts

### AI Notes Summarizer (`artifacts/notes-summarizer`)
- React + Vite frontend at `/`
- Dark-themed UI with file upload, text paste, AI summarize, and Q&A
- Falls back to dummy output if AI API is unavailable

### API Server (`artifacts/api-server`)
- Express backend at `/api`
- Routes:
  - `GET /api/healthz` — health check
  - `POST /api/notes/summarize` — summarize text with AI (returns bullet points)
  - `POST /api/notes/ask` — answer a question about the text

## Key Commands

- `pnpm run typecheck` — full typecheck across all packages
- `pnpm run build` — typecheck + build all packages
- `pnpm --filter @workspace/api-spec run codegen` — regenerate API hooks and Zod schemas from OpenAPI spec
- `pnpm --filter @workspace/db run push` — push DB schema changes (dev only)
- `pnpm --filter @workspace/api-server run dev` — run API server locally

See the `pnpm-workspace` skill for workspace structure, TypeScript setup, and package details.
