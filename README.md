# AppRun Agent Skill

This repository contains an agent skill for AI coding assistants focused on developing AppRun applications in TypeScript with the MVU (Model-View-Update) pattern. The skill covers component patterns, event handling, state management (including async generators), routing and navigation with parameters and guards, and testing with Vitest.

## What's Included

- **Project Setup**: Vite configuration, TypeScript setup, and recommended folder structure
- **Component Patterns**: Stateful class components, modal components, functional components, and typed events
- **Event System**: AppRun directives (`$bind`, `$onclick`, etc.) and event communication patterns
- **State Management**: Update handlers (sync, async, generators), state initialization rules
- **Routing**: Component registration, navigation, route parameters, and programmatic routing
- **Testing**: Unit testing patterns with Vitest
- **Development Checklist**: Complete checklist for building AppRun components

## Install the Skill

### Recommended: install with `npx skills`

Use the `skills` CLI to install this repository as an agent skill:

```bash
npx skills add yysun/apprun-skills
```

Useful variations:

```bash
# Install globally instead of in the current project
npx skills add yysun/apprun-skills --global

# Install to a specific agent only
npx skills add yysun/apprun-skills --agent github-copilot

# Preview what the repository exposes
npx skills add yysun/apprun-skills --list
```

### Manual installation

If you do not want to use `npx skills`, create an `apprun-skills` folder in your agent's skills directory and place this repository's `SKILL.md` inside it.

Example:

```text
.agents/skills/apprun-skills/SKILL.md
```

Current skill directories for common coding agents:

| Agent | Project install folder | Global install folder |
|---|---|---|
| Claude Code | `.claude/skills/apprun-skills/` | `~/.claude/skills/apprun-skills/` |
| Cursor | `.agents/skills/apprun-skills/` | `~/.cursor/skills/apprun-skills/` |
| GitHub Copilot | `.agents/skills/apprun-skills/` | `~/.copilot/skills/apprun-skills/` |
| Cline | `.agents/skills/apprun-skills/` | `~/.agents/skills/apprun-skills/` |
| OpenAI Codex | `.agents/skills/apprun-skills/` | `~/.codex/skills/apprun-skills/` |
| Windsurf | `.windsurf/skills/apprun-skills/` | `~/.codeium/windsurf/skills/apprun-skills/` |

Project installs keep the skill in the repository. Global installs make it available across all projects for that agent.

## License

MIT License - see LICENSE file for details
