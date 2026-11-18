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

## Plank AI FDE Course

Your project for Plank's [AI FDE Course](https://joinplank.com/ai-fde-course).

One repository for the whole course. Day 1 scaffolds it, and every day after
adds to it: WorkBot, an enterprise workflow platform, grows here week by week.
There are no per-day folders. The project is the deliverable.

## How verification works

When you finish a day, open the day's page in the course and press
**Verify Day N**. Plank reads this public repository (it never writes to it)
and checks whether the commits since your last verified day are broadly that
day's work. What the day ships is the yardstick, and partial progress counts.
Days verify in order.

Keep commits small and messages honest. They are what the check reads.

## Structure

Yours to decide. From Week 6 the course moves WorkBot into a config-first
monorepo, so a layout with room for several apps and shared packages saves a
move later.

## Your profile

Every verified day appears on your public profile at
`joinplank.com/fde/<your-github-login>`, with what you shipped and the skills
it added. The repository description links to it; add the same link as the
repository's website so it shows under the name.
