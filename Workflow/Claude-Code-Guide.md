# Claude Code Guide

Reference for using Claude Code in VSCode. Keep this updated as you learn.

---

## Modes

Cycle modes with **Shift+Tab**:

| Mode         | Shortcut         | What it does                                      | When to use                        |
|--------------|------------------|---------------------------------------------------|------------------------------------|
| Normal       | Default          | Asks approval before every edit/command           | Default — always start here        |
| Auto-Accept  | Shift+Tab × 1    | Applies changes automatically, no prompts         | Only after reviewing a clear plan  |
| Plan         | Shift+Tab × 2    | Read-only — explores codebase, writes plans only  | First step of every feature        |

> Tip: The mode indicator shows at the bottom of the Claude terminal panel.

---

## Key Shortcuts

| Shortcut         | Action                              |
|------------------|-------------------------------------|
| Shift+Tab        | Cycle through modes                 |
| /clear           | Reset conversation context          |
| /model           | Switch model (Sonnet / Opus)        |
| Esc              | Cancel current input                |
| Enter            | Send message                        |

---

## Recommended Starting Prompts

**Planning a feature:**
```
Read CLAUDE.md and obsidian/ folder.
Plan implementation for [JOB-X]: [feature description]
List the steps without writing any code yet.
```

**Starting implementation:**
```
Implement step 1 from the plan.
Ask me before moving to the next step.
```

**Debugging:**
```
Read the error below and suggest a fix without changing anything yet.
[paste error]
```

**Refactoring:**
```
Read [file]. Suggest refactors for readability and TypeScript best practices.
Do not change logic.
```

---

## Model Choice

- **Sonnet 3.7** → Fast, good for most tasks (components, fixes, refactors)
- **Opus** → Complex reasoning, architecture planning, tricky bugs

---

## Tips

- Always start with Plan Mode for new features — never jump straight to code
- Use `/clear` between unrelated tasks to avoid context pollution
- Keep CLAUDE.md in every project repo updated — it's Claude's memory
- Reference Obsidian notes in your prompt: *"Check obsidian/ for context on X"
- Small steps > big steps: ask Claude to do one thing at a time

---

See also: [[Dev-Workflow]]
