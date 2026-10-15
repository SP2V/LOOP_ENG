# Claude Engineering Team V2 — Mandatory Development Loop

Claude Code configuration with an orchestrator skill, 8 specialist agent definitions, and a mandatory development loop for new and modified modules.

## Install
1. Unzip the archive.
2. Copy `CLAUDE.md`, `.claude/`, and optionally `docs/` into the **root of your repository**.
3. If your project already has `CLAUDE.md`, **merge** the V2 loop and safety rules instead of overwriting project-specific instructions.
4. Start Claude Code from the repository root. Ask: `Use the engineering-team skill to implement [feature]. Follow the mandatory development loop and report verification evidence.`
5. Check that Claude actually reads project instructions and performs the steps; skills may be invoked according to tool/version behavior. The root `CLAUDE.md` makes the loop the default.

## Included
- `CLAUDE.md` — default rules and mandatory development loop
- `.claude/skills/engineering-team/SKILL.md` — orchestrator skill
- `.claude/agents/*.md` — architect, frontend, backend, database, devops, security, qa, reviewer
- `docs/DEVELOPMENT_LOOP.md` — diagram, checklist, reporting template
- `docs/TASK_TEMPLATE.md` — task template

## Operational boundaries
This does not grant privileges, bypass approvals, guarantee agent delegation, or guarantee error-free code. Production/destructive changes require approval. No automatic commit/push/deploy by default.
"# LOOP_ENG" 
