# Guide to the 0softwaredevelopment0 Organization

This guide explains how the **0softwaredevelopment0** organization is put together, what projects we maintain, and how everything stays consistent across the organization. It applies to **all** repositories equally.

For *contributing* to the code, see our [Contributing Guide](CONTRIBUTING.md). For security matters, see the [Security Policy](SECURITY.md).

---

## Table of Contents

- [Who We Are](#who-we-are)
- [Our Projects](#our-projects)
- [How Projects Are Organized](#how-projects-are-organized)
- [Common Conventions](#common-conventions)
  - [Licensing](#licensing)
  - [Documentation](#documentation)
  - [Portability](#portability)
  - [Build Systems](#build-systems)
- [Getting Started](#getting-started)
- [Where to Ask for Help](#where-to-ask-for-help)

---

## Who We Are

We build open-source tools and plugins. Some are desktop utilities (portable, single-file), some are Minecraft server plugins, and some are web-based. The common thread: everything is **open source**, **self-contained**, and maintained under one roof so behavior and conventions stay consistent.

---

## Our Projects

| Project | Type | Description |
|---------|------|-------------|
| **RustLauncher** | Desktop (Rust) | Minecraft launcher with instances and a Modrinth browser |
| **SoundPad** | Desktop (Rust) | Play sound effects / audio files |
| **IpParser** | Desktop (Rust) | Regex/CIDR IP & port scanner with Minecraft probe |
| **UltraMonitor** | Desktop (Rust) | Hardware monitoring and stress tests |
| **DirectMessages** | Desktop (Rust) | Encrypted peer-to-peer messenger over TCP |
| **OrganizationWebsite** | Web (TypeScript) | Organization website |
| **UltimateImprovments** | Minecraft plugin | Big feature plugin (tech, security, achievements) |
| **CubixSMP** | Minecraft plugin | Essentials plugin for the Cubix server |
| **ShiftBypass** | Minecraft mod | Small Fabric mod that unblocks Shift in some screens |
| **PingSpoof** | Minecraft mod | Small Fabric mod that sets a custom ping |
| **NPPsim** | Desktop (Rust) | Nuclear power plant control simulator |
| **TheMinesweeper** | Desktop (Rust) | Minesweeper game with much more functionality than the original |
| **... and more** | — | New projects are added under the same conventions |

Check the organization page for the full up-to-date list: [0softwaredevelopment0](https://github.com/0softwaredevelopment0).

---

## How Projects Are Organized

Every repository in this organization follows the same structure so you always know where to look:

- **`README.md`** — what the project is, install/run instructions, and links.
- **`LICENSE`** — AGPLv3 license text.
- **`src/main/java/`** (backends / servers) or **`src/`** (frontend) — the actual code.
- **`build/`** — build output (not committed).
- **`logs/`, `data/`, runtime files** — generated at runtime, kept **outside** the repo.

Project-specific documentation that is not shown by GitHub in the sidebar (plans, guides, changelogs, test plans) lives directly inside each repository, next to the code it describes. Shared, organization-wide policies live in this `.github` repository so they can be edited in one place and apply everywhere.

---

## Common Conventions

### Licensing

All projects are licensed under the **GNU Affero General Public License v3.0 (AGPLv3)**. New projects must use the same license so the whole organization stays consistent.

### Documentation

- Every repository has a clear `README.md`.
- Shared policies (contributing, security, code of conduct) are kept in `.github`.
- Project-specific docs (usage guides, changelogs, plans) live with the code.

### Portability

Desktop tools are designed to run **portably** — no global installs, no leftover files on the system. Runtime files (logs, databases) are written into a directory the launcher controls, and `logs/` holds per-run log files.

### Build Systems

| Project type | Build tool |
|--------------|-----------|
| Java (Gradle) | Gradle (`./gradlew build`) |
| Rust | Cargo (`cargo build --release`) |
| Web (TypeScript) | npm (`npm install && npm run dev`) |
| Minecraft plugins | Gradle multi-module |

---

## Getting Started

1. Pick a project from the [organization page](https://github.com/0softwaredevelopment0).
2. Read its `README.md` for install/run instructions.
3. For desktop tools, download the portable build and run its launcher — no installation needed.

---

## Where to Ask for Help

- **Questions:** ask in [Discussions](https://github.com/0softwaredevelopment0/.github/discussions) — use the **Q&A** category for anything with a clear answer.
- **Bugs & feature requests:** open an Issue in the specific repository (use the issue templates).
- **Contributing:** see [CONTRIBUTING.md](CONTRIBUTING.md).
- **Security vulnerabilities:** see [SECURITY.md](SECURITY.md) — report privately, never in a public Issue.

---

Thank you for being part of 0softwaredevelopment0!