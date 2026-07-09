# CLAUDE.md

Guidance for Claude Code (and any AI assistant) working in this repository.

## Project Overview

Capstone project for the Frontend AI Engineering track. *(Add a 2-3 sentence description of what the app actually does once scoped.)*

## Tech Stack

- **Framework:** React (functional components + hooks only, no class components)
- **Build tool:** Vite
- **Runtime:** Node.js (LTS)
- **Package manager:** npm
- **Language:** JavaScript *(switch this line to TypeScript if you adopt it later)*

## Commands

| Command | Purpose |
|---|---|
| `npm run dev` | Start local dev server |
| `npm run build` | Production build |
| `npm run preview` | Preview the production build locally |
| `npm run lint` | Run linter |
| `npm test` | Run tests *(once a test runner is added, e.g. Vitest)* |

## Conventions

**Components**
- One component per file, PascalCase filenames (`UserCard.jsx`)
- Functional components with hooks; avoid unnecessary `useEffect`
- Co-locate component-specific styles/tests next to the component

**Naming**
- Components: `PascalCase`
- Functions/variables: `camelCase`
- Constants: `UPPER_SNAKE_CASE`

**Folder structure**
- `src/components/` — reusable, presentational components
- `src/pages/` — route-level views
- `src/hooks/` — custom hooks
- `src/assets/` — static files

**Commits**
- Follow [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/): `type(scope): description`
- Common types: `feat`, `fix`, `docs`, `chore`, `refactor`, `test`

**Styling**
- *(Fill in once decided — e.g. CSS Modules, Tailwind, styled-components)*

## What Claude Should Do

- Prefer small, focused commits with clear Conventional Commit messages
- Explain non-obvious code changes briefly before applying them
- Keep components small and composable; flag when a file is growing too large

## What Claude Should NOT Do

- Don't install new dependencies without asking first
- Don't rewrite unrelated files while fixing a specific bug
- Don't remove existing comments/tests without confirming they're safe to drop
