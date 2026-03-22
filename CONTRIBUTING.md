# Contributing to Codnov

## Getting Started

1. Clone the repo
2. Install dependencies: `npm ci`
3. Create a feature branch from `main`
4. Make your changes
5. Submit a Pull Request

## Branch Naming

| Type | Pattern | Example |
|------|---------|---------|
| Feature | `feat/short-description` | `feat/add-contact-form` |
| Bug fix | `fix/short-description` | `fix/login-redirect` |
| Chore | `chore/short-description` | `chore/update-deps` |

## Commit Messages

Use clear, imperative commit messages:

```
feat: add client pipeline dashboard view
fix: resolve 401 redirect loop on token expiry
chore: update Next.js to 15.5
```

Prefix with: `feat:`, `fix:`, `chore:`, `refactor:`, `test:`, `docs:`, `ci:`

## Pull Requests

- Keep PRs focused — one feature or fix per PR
- PR title should be under 70 characters
- Fill in the PR template completely
- CI must pass before requesting review
- All PRs require approval from `@nidin-cyber`

## Code Standards

- **TypeScript** — strict mode, no `any` unless justified
- **Tailwind CSS** — no CSS modules, styled-components, or inline styles
- **API calls** — always use the shared Axios instance from `src/lib/api.ts`
- **State** — Zustand for global state, React Hook Form + Zod for forms
- **No secrets in code** — use environment variables

## What Not to Do

- Do not push directly to `main`
- Do not commit `.env` files or secrets
- Do not use `fetch()` — use the Axios instance
- Do not add backend logic to frontend repos
- Do not hardcode API URLs
