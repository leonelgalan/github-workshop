# Git & GitHub Workshop

Two-session hands-on workshop teaching Git and GitHub fundamentals through
collaborative data analysis.

## Workshop Overview

**Audience:** Master of Science in Analytics students
**Duration:** Two 75-minute sessions (Tuesday & Friday)
**Format:** Interactive slides with live coding and group exercises

## Learning Objectives

1. Understand version control concepts and Git workflow
2. Use Git locally (commit, branch, merge, rebase)
3. Collaborate via GitHub (fork, clone, pull requests, code review)
4. Resolve merge conflicts professionally
5. Apply Git best practices to real analytics projects

## Workshop Project

Students collaborate on a movie ratings analysis pipeline:

- **Session 1:** Groups of 4 implement functions in a data cleaning script,
  submit PRs
- **Between Sessions:** Complete assigned analysis scripts (genre trends,
  financials, or modeling)
- **Session 2:** Integrate all work, resolve conflicts, run complete pipeline

Project repository: [leonelgalan/movie-analysis](https://github.com/leonelgalan/movie-analysis)

## Slides

Built with [Slidev](https://sli.dev/) for a modern, code-friendly presentation experience.

### Running the Slides

```bash
pnpm install
pnpm run dev
```

Open <http://localhost:3030> to view the presentation.

### Building for Production

```bash
pnpm run build
```

Outputs to `dist/` directory.

## Content Structure

- `slides.md` — Main slide deck entry point
- `pages/` — Individual slide sections:
  - `00-intro.md` — Workshop introduction
  - `01-why.md` — Why version control matters
  - `02-tools.md` — Git, GitHub, VS Code setup
  - `03-terminal.md` — Essential terminal commands
  - `04-demo.md` — Live Git demonstration
  - `05-project.md` — Group project instructions

## Resources

- [Full project specification](https://github.com/leonelgalan/movie-analysis/blob/main/docs/SPEC.md)
- [Slidev documentation](https://sli.dev/)
- [Git documentation](https://git-scm.com/doc)
