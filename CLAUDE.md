# Global Claude Context

## Identity
- Name: Mohammad Maleh
- Location: Munich, Germany
- Email: mohammad.maleh@gmail.com

## Workflow Stack
- Research: Perplexity AI → save to obsidian/research/
- Notes: Obsidian (this vault) → auto-synced to GitHub
- PM: Linear (cloud, free)
- Dev: VSCode + Claude Code (WSL Ubuntu)
- Version Control: GitHub
- UI/UX: TBD

## Active Projects

### job-tracker
- **What**: Personal web app to track job applications (add, update, monitor status)
- **Repo**: https://github.com/mohammadmaleh/job-tracker (local: ~/projects/job-tracker)
- **Stack**: React 18 + Vite + TypeScript + Tailwind CSS
- **Linear**: Job Application Tracker (issue prefix: JOB-X)
- **Status**: 🟡 In Progress — Vite + Tailwind skeleton done, UI components not yet connected
- **Structure**: `frontend/` → Vite app → `src/App.tsx`, `main.tsx`
- **Next steps**: Define TypeScript data model, build job list view, add/edit form, status tracking
- **Full context**: See `projects/job-tracker/README.md` in this vault

## Vault Structure
- research/ → Perplexity research dumps
- projects/ → per-project notes (e.g. projects/job-tracker/README.md)
- daily/ → daily notes
- Workflow/ → workflow setup
- Tech/ → tech notes

## Global Dev Rules
- No self-hosted DevOps, keep it lightweight
- Always create a Linear issue before coding
- Branch format: feat/JOB-X-description
- Commit format: "feat: description JOB-X"
- PR title must reference Linear issue

## How to Use This Vault
- Read CLAUDE.md first every session
- Check projects/<project-name>/README.md for active context
- Write research findings to research/YYYY-MM-DD-topic.md
- Update daily/YYYY-MM-DD.md with progress
