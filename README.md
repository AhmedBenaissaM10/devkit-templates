# devkit-templates

Reusable, non-runnable templates and reference material for backend projects built with **TypeScript, Express, and Prisma**.

This is not a starter project you clone and run — it's a personal toolkit of copy-pasteable configs, boilerplate snippets, and cheatsheets, kept up to date as I learn better practices.

## Why this exists

Every new project starts with the same setup: linting, Docker, CI/CD, test scaffolding, error handling patterns. Instead of rewriting or hunting these down each time, this repo centralizes them in one place, organized by category.

## Structure

```
devkit-templates/
├── config/           # tsconfig, ESLint, Prettier, vitest, editorconfig, env schema
├── docker/           # Dockerfile, docker-compose (dev/prod), .dockerignore
├── github/           # CI/CD workflows, issue & PR templates, CODEOWNERS, dependabot
├── tests/            # setup, mocks, helpers, sample test structure
├── snippets/         # AppError, catchAsync, logger, Prisma schema/seed templates
├── docs-templates/   # README, CONTRIBUTING, ARCHITECTURE skeletons
└── cheatsheets/       # git, docker, prisma, express, typescript, postgres, bash, regex
```

## How to use

Browse the relevant folder, copy the file(s) you need into your project, and adjust for context. Each folder has its own short `README.md` explaining what's inside and any setup notes.

## Contents

| Folder | What's inside |
|---|---|
| `config/` | tsconfig variants, ESLint flat config, Prettier, vitest config, `.env.example` + schema, package.json scripts template |
| `docker/` | Multi-stage Dockerfile, dev/prod compose files, `.dockerignore`, healthcheck snippet |
| `github/` | `ci.yml`, `cd.yml`, `ci_cd.yml`, PR/issue templates, dependabot config |
| `tests/` | Global test setup, Prisma mocks, auth/test-data helpers, sample test file |
| `snippets/` | Centralized error handling (`AppError`, `catchAsync`), logger config, Prisma schema/seed templates |
| `docs-templates/` | README skeleton, CONTRIBUTING, ARCHITECTURE (vertical-slice pattern) |
| `cheatsheets/` | Quick-reference `.md` notes for git, Docker, Prisma, Express, TypeScript, PostgreSQL, bash, regex |

## Conventions followed

- Feature-based (vertical slice) architecture
- Thin controllers, fat services
- Centralized error handling (`AppError` + `catchAsync`)
- Env validation at startup
- Conventional commits (via commitlint + husky)

## Status

🚧 Actively maintained — updated as I refine practices across projects.

## License

MIT

