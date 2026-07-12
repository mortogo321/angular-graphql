# Angular + Express Monorepo Starter

A two-module starter pairing an Angular frontend with an Express REST API — a baseline scaffold for wiring up a full-stack TypeScript/JavaScript project before adding real domain logic.

## What's inside

- `api/` — an Express REST API starter (based on the `express-api-starter` template) with request logging (morgan), security headers (helmet), env config (dotenv), and a sample `/api/v1/emojis` endpoint. Includes ESLint, Mocha/Supertest tests, and a Snyk audit script.
- `web/` — an Angular CLI-generated frontend scaffold (default starter app, unmodified beyond project setup), including unit tests (Karma/Jasmine) and e2e tests (Protractor).

Note: despite the repository name, no GraphQL or MongoDB integration is currently implemented in either module — both are presently REST/starter-level scaffolds.

## Tech stack

**API**
- Express, morgan, helmet, dotenv
- ESLint, Mocha, Supertest, Snyk (dev/test tooling)

**Web**
- Angular, RxJS
- Karma/Jasmine (unit tests), Protractor (e2e tests)

## Project structure

```
api/     Express REST API
web/     Angular application
```

## Quickstart

Each module has its own dependencies and lockfile (`yarn.lock`).

### API

```
cd api
yarn install
cp .env.sample .env
yarn dev
```

### Web

```
cd web
yarn install
yarn start
```

Then open http://localhost:4200.

## Endpoints (API)

- `GET /` — health/welcome message
- `GET /api/v1` — API root message
- `GET /api/v1/emojis` — sample emoji list
