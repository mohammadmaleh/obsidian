# Default Dev Workflow

This is my standard workflow for every project. Stack: **Claude + VSCode + Obsidian + Linear + Penpot**.

---

## Tools & Roles

| Tool       | Role                                      |
|------------|-------------------------------------------|
| Linear     | Task/issue tracking (PM)                  |
| Penpot     | UI/UX design & developer handoff          |
| VSCode     | Code editor                               |
| Claude     | AI pair programmer inside VSCode          |
| Obsidian   | Knowledge base, project notes, planning   |

---

## End-to-End Flow

### 1. Idea / Feature Request
- Capture the idea as a note in `projects/<project-name>/`
- Outline goals, acceptance criteria, and open questions
- Use Claude in Plan Mode to refine: *"Read this note and help me break it into Linear issues"

### 2. Design (if UI involved)
- Open Penpot → design the feature/screen
- Export specs (CSS, spacing, tokens) from the Inspect panel
- Save Penpot link in the Linear issue description

### 3. Linear Issue
- Create a Linear issue **before writing any code**
- Add: description, acceptance criteria, Penpot link (if applicable)
- Assign priority and label (feature / bug / chore)
- Issue is auto-prefixed: `JOB-X`, `APP-X`, etc.

### 4. Branch
- Create branch directly from Linear (auto-naming: `feat/JOB-X-description`)
- Check out locally: `git checkout feat/JOB-X-description`

### 5. Plan with Claude
- Open VSCode Claude panel
- Switch to **Plan Mode** (Shift+Tab twice)
- Prompt: *"Read CLAUDE.md and obsidian/ folder. Plan implementation for [JOB-X]: [feature description]"
- Review the plan, adjust if needed

### 6. Implement
- Switch to **Normal Mode** (Shift+Tab back)
- Work step by step with Claude: approve each change
- Use **Auto-Accept** only for low-risk mechanical tasks
- `/clear` to reset context between logical steps

### 7. Commit
- Format: `feat: description JOB-X`
- Example: `feat: add job card component JOB-4`
- Push branch: `git push origin feat/JOB-X-description`

### 8. Pull Request
- Open PR → link to Linear issue ("Closes JOB-X")
- Linear auto-moves ticket to Done on merge

### 9. Document
- Update relevant note in `projects/<project-name>/`
- Capture learnings in `projects/<project-name>/Learnings.md`

---

## Commit Message Convention

```
feat: short description JOB-X     → new feature
fix: short description JOB-X      → bug fix
chore: short description JOB-X    → maintenance
refactor: short description JOB-X → refactoring
docs: short description           → documentation only
```

---

## Rules
- Always create a Linear issue **before** coding
- Always start with **Plan Mode** before touching code
- Keep obsidian project notes updated — Claude reads them
- Link Penpot designs in Linear issue before implementing UI

---

See also: [[Claude-Code-Guide]]
