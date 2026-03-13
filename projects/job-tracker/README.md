# Job Tracker

## Overview
A personal web app to track job applications throughout a job search. The goal is a single, clean dashboard where Mohammad can add, update, and monitor every application — from first contact to offer or rejection.

## Status
🟡 In Progress — Vite + Tailwind skeleton is set up, UI components not yet connected.

## Repo
- GitHub: https://github.com/mohammadmaleh/job-tracker
- Local: ~/projects/job-tracker
- Linear: Job Application Tracker (issue prefix: JOB-X)

## Tech Stack
| Layer | Choice |
|---|---|
| Framework | React 18 |
| Build Tool | Vite |
| Language | TypeScript |
| Styling | Tailwind CSS |
| Package Manager | npm |

## Repo Structure
```
job-tracker/
└── frontend/         ← Vite + React app
    ├── src/
    │   ├── App.tsx
    │   ├── App.css
    │   ├── main.tsx
    │   └── index.css
    ├── index.html
    ├── vite.config.ts
    ├── tsconfig.json
    └── package.json
```

## Progress Checklist
- [x] Vite + React + TypeScript scaffold
- [x] Tailwind CSS configured
- [ ] Job application data model (TypeScript types)
- [ ] Add/edit job application form
- [ ] Application list/table view
- [ ] Status tracking (Applied, Interview, Offer, Rejected)
- [ ] Filtering and sorting
- [ ] Persistence (localStorage or backend TBD)
- [ ] Deployment (Vercel)

## Dev Conventions
- Always create a Linear issue before writing code (prefix: JOB-X)
- Branch format: `feat/JOB-X-short-description`
- Commit format: `feat: description JOB-X`
- PR title must reference the Linear issue
- No self-hosted DevOps — keep everything lightweight

## Open Questions / Decisions Pending
- Backend? (options: none/localStorage, Supabase, or lightweight Node API)
- Auth? (probably not needed for v1 — personal use only)
- Deployment target: Vercel (frontend-only for now)
