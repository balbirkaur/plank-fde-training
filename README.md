# WorkBot Enterprise AI

WorkBot is an enterprise AI application built with Next.js, React, and TypeScript.

## Prerequisites

- Node.js 20.x
- pnpm 10.34.9 (pinned in `package.json`)

If pnpm is not installed, install the pinned version with npm:

```powershell
npm install --global pnpm@10.34.9
```

## Install and run locally

Install the dependencies and start the development server:

```powershell
pnpm install
pnpm dev
```

Open [http://localhost:3000](http://localhost:3000) to view the app. The app
uses the Next.js App Router under `src/app`.

## Quality checks and production build

Run the repository quality checks before opening a pull request:

```powershell
pnpm check
```

This checks Prettier formatting, ESLint rules, and TypeScript types. To format
files locally, run `pnpm format`. To create and run the production build:

```powershell
pnpm build
pnpm start
```

GitHub Actions runs `pnpm check` and `pnpm build` for pull requests targeting
`main` and pushes to `main`.

## Package manager

Use pnpm for dependency installation and updates. `pnpm-lock.yaml` is the
canonical lockfile. `package-lock.json` is retained temporarily and should not
be used to install or update dependencies.
