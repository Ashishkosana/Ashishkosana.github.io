# E-commerce Site — Refactor Brief

*(Handoff note for a future Claude Code session. This is a local note — gitignore or delete anytime.)*

## What this is
My **business e-commerce website**. I originally built it with ChatGPT *before* I had real
engineering experience. It's fully functional, but I now want to refactor it to **industry
best practices**, using everything I've learned working at Crewtron. This is a "level it up
properly" project — not a rewrite-from-scratch.

## Goal for the dedicated session
1. **Audit first** — current structure, stack, and the main gaps: architecture, security,
   secrets handling, testing, CI/CD, performance, accessibility, SEO, error handling.
2. **Plan in phases** — a prioritized, phased refactor that keeps the site working throughout.
3. **Execute** phase by phase, with my review at each step.

## ⚠️ My environment & identity (read before doing anything)
- **Default browser = Safari = CREWTRON (work).** Do **not** use Safari / the default browser
  for this project.
- **Firefox = PERSONAL.** All my personal accounts live in Firefox: **GitHub (`Ashish1916`)**,
  **Vercel**, and everything tied to my personal projects.
- 👉 **For this project, use Firefox for anything browser-based** — OAuth logins, `vercel login`,
  deploy/preview URLs, dashboards. When opening a link from the terminal, open it in Firefox
  explicitly: `open -a Firefox "<url>"`.
- **CLI identities (personal):**
  - GitHub: `gh auth switch --user Ashish1916`  (work account is `ashishk-crewtron`).
  - AWS (only if needed): `export AWS_PROFILE=personal`  (personal account `921888034384`).
    NOTE: both `ashish` and `crewtron-beta` AWS profiles are **Crewtron** — never use them here.
  - Anything under `~/projects/` auto-commits as my personal email via a git `includeIf`.
- **Hosting:** Vercel (personal account, logged in via Firefox). *(Confirm at session start —
  the repo is named `*.github.io` but I deploy via Vercel.)*

## Where it lives
`~/projects/Ashish1916.github.io`

## First steps when we start
1. Confirm personal identity: `gh auth status` → `Ashish1916` active.
2. Audit the repo (stack, dependencies, structure, secrets, tests, CI).
3. Present a **phased refactor plan for my approval** before changing anything.
