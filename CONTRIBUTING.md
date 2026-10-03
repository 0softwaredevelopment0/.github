# Contributing to 0softwaredevelopment0

Thank you for your interest in contributing! This guide applies to all repositories under the **0softwaredevelopment0** organization and explains how to ask for help, report bugs, suggest features, and submit code.

Whether you're fixing a typo or building a whole new module — you're welcome here, and every legitimate contribution counts.

---

## Table of Contents

- [Code of Conduct](#code-of-conduct)
- [Getting Help — Questions & Discussions](#getting-help--questions--discussions)
- [Finding Something to Work On](#finding-something-to-work-on)
- [How to Contribute](#how-to-contribute)
  - [Reporting Bugs](#reporting-bugs)
  - [Suggesting Features](#suggesting-features)
  - [Submitting Code](#submitting-code)
- [Pull Request Guidelines](#pull-request-guidelines)
- [Commit Message Guidelines](#commit-message-guidelines)
- [Code Style](#code-style)
- [Development Setup](#development-setup)
- [Before You Submit — Checklist](#before-you-submit--checklist)
- [License & Contribution Agreement](#license--contribution-agreement)

---

## Code of Conduct

Please read our [Code of Conduct](CODE_OF_CONDUCT.md). Be respectful, constructive, and kind in Issues, Discussions, and Pull Requests. Harassment, trolling, and spam are not tolerated.

---

## Getting Help — Questions & Discussions

**Before opening an Issue, please ask questions in Discussions.** Discussions are the right place for:

- "How do I configure X?"
- "What does this command / feature do?"
- "Why isn't Y working on my server / setup?"
- General usage help and ideas.

> **Tip:** use the **Q&A** category for questions that have a clear answer. Mark the best answer as **accepted** when it helped you — it makes the answer easy to find for everyone else, and it's how the community keeps good answers discoverable.

- **Start a Discussion:** [0softwaredevelopment0 Discussions](https://github.com/0softwaredevelopment0/.github/discussions)
- **Chat with us live:** [Discord](https://dsc.gg/rizer001-Development)

Use **Issues** only for concrete, actionable problems (bugs) or well-scoped feature requests — see below.

---

## Finding Something to Work On

Not sure where to start? Try:

1. Browse the [repositories](https://github.com/0softwaredevelopment0) and pick one that interests you.
2. Look for open Issues tagged `good first issue`, `help wanted`, or `enhancement`.
3. Check active pull requests to avoid duplicating someone else's work.
4. Ask in Discussions/Discord if a feature is already planned before you invest time.

---

## How to Contribute

### Reporting Bugs

Bugs should be reported as Issues. To help us fix them fast:

- Search existing Issues and Discussions first — it may already be reported.
- Open an Issue in the **relevant repository** (not in `.github`).
- Use the **Bug Report** template when available.
- Include:
  - **Steps to reproduce**
  - **Expected vs. actual behavior**
  - **Environment**: OS, Java version, loader/mod/plugin version, Minecraft/Paper version where applicable
  - **Screenshots or logs** if they help
- One bug per issue, please.

### Suggesting Features

- Describe the **problem you're trying to solve**, not just the solution.
- Explain why this feature would be useful to others.
- If the scope is large or ambiguous, start a **Discussion** first; if it's a clear, small addition, open an Issue.
- Check whether it's already planned to avoid duplicates.

### Submitting Code

1. **Fork** the repository.
2. **Create a branch** from `main`:
   ```bash
   git checkout -b feature/your-feature-name
   ```
   Use a name that summarizes the work (e.g. `fix/config-reload`, `feat/new-command`).
3. **Make focused changes** — small, reviewable commits with descriptive messages.
4. **Format the code** according to the project's style (see [Code Style](#code-style)).
5. **Build and test** locally before submitting (see [Development Setup](#development-setup)).
6. **Keep `main` up to date** — rebase or merge the latest upstream before pushing.
7. **Push** to your fork and open a **Pull Request** against `main`.

---

## Pull Request Guidelines

- **Clear title** — imperative and specific, e.g. "Fix crash when loading an empty sound file".
- **Link the issue** it fixes, e.g. `Closes #42`.
- **Describe what changed and why** in the description.
- **Keep it focused** — one feature or fix per PR. Large changes are easier to review when split.
- **Run the build** and any tests before submitting.
- **Respond to review feedback** promptly.

We review PRs in order of submission and will try to get to yours quickly. Minor feedback is normal — it's not a rejection.

---

## Commit Message Guidelines

Well-written history makes the project easier to understand and maintain:

- Use **imperative mood**: "Fix bug" not "Fixes bug" / "Fixed bug".
- Keep the **first line under ~72 characters**.
- Add a short body explaining *why* when it isn't obvious.
- Reference issues when applicable: `Fix crash on empty input (#12)`.

Example:

```
Fix NPE when config is missing the homes section

The homes map was accessed before ensuring it existed, throwing on first
login. Initialise it on load.

Closes #8
```

---

## Code Style

| Project | Language | Style |
|---------|----------|-------|
| Java projects | Java | Standard Java conventions (Google Java Style or project-specific `.editorconfig`) |
| Rust projects | Rust | `cargo fmt` + `cargo clippy` clean |
| OrganizationWebsite | TypeScript | The project's ESLint/Prettier config |

When in doubt, match the surrounding code in the repository you're editing.

---

## Development Setup

Each project has its own build system:

| Project / Type | Build Tool | Command |
|---------|-----------|---------|
| Java (Gradle) | Gradle | `./gradlew build` |
| Rust projects | Cargo | `cargo build --release` |
| OrganizationWebsite | npm | `npm install && npm run dev` |

Make sure you have the required toolchain installed: **JDK 21+** for Java projects (some need a newer LTS — check the project README) or a current **Rust** toolchain for Rust projects.

---

## Before You Submit — Checklist

- [ ] I searched existing Issues/Discussions and this isn't a duplicate.
- [ ] My change is focused on a single bug/feature.
- [ ] The code follows the project's style.
- [ ] I built the project successfully.
- [ ] I ran the relevant tests (if any).
- [ ] My PR description explains *what* and *why*.
- [ ] I referenced the issue(s) it closes, if any.

---

## License & Contribution Agreement

All projects in this organization are licensed under the **GNU Affero General Public License v3.0 (AGPLv3)**.

By submitting a contribution, you agree that your work will be licensed under the same **AGPLv3** license as the project you're contributing to.

> AGPLv3 is **copyleft and network-interactive**: modifications must stay open-source, and if you run a modified version as a service, you must offer the source to its users. Make sure you're comfortable with this before contributing.

---

## Still Stuck?

- **Discussions:** [0softwaredevelopment0 Discussions](https://github.com/0softwaredevelopment0/.github/discussions)
- **Discord:** [Join our server](https://dsc.gg/rizer001-Development)
- **Email:** [dan.al.zhu@gmail.com](mailto:dan.al.zhu@gmail.com)

Thank you for helping make the 0softwaredevelopment0 projects better!