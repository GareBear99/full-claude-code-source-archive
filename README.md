<div align="center">

# Gary Doman’s Claude Code Source Archive

**Public-facing source archive, architecture index, and MCP exploration toolkit curated by Gary Doman ([GareBear99](https://github.com/GareBear99))**

[![TypeScript](https://img.shields.io/badge/TypeScript-512K%2B_lines-3178C6?logo=typescript&logoColor=white)](#tech-stack)
[![Bun](https://img.shields.io/badge/Runtime-Bun-f472b6?logo=bun&logoColor=white)](#tech-stack)
[![MCP Server](https://img.shields.io/badge/MCP-Explorer_Server-blueviolet)](#mcp-server)
[![Maintainer](https://img.shields.io/badge/Maintainer-Gary_Doman-111827)](https://github.com/GareBear99)

</div>

## What this repository is

This repository is a **public source archive and documentation hub** for a Claude Code TypeScript source snapshot, reorganized for easier exploration, search visibility, and developer readability by **Gary Doman / GareBear99**.

It is designed for people searching for:

- Claude Code source archive
- Claude Code architecture
- Claude Code tools and commands
- Claude Code MCP explorer
- TypeScript CLI architecture analysis
- Claude Code reverse engineering notes

## Why this repo is useful

Instead of acting like a raw dump, this version is positioned as a **developer research repo** with:

- architecture notes
- command and tool references
- subsystem breakdowns
- MCP server support for interactive exploration
- documentation surfaces tuned for public GitHub discoverability

## Maintainer

**Gary Doman**  
GitHub: [GareBear99](https://github.com/GareBear99)

---

## Table of Contents

- [What this repository is](#what-this-repository-is)
- [Why this repo is useful](#why-this-repo-is-useful)
- [What is Claude Code?](#what-is-claude-code)
- [Repository Highlights](#repository-highlights)
- [Documentation](#documentation)
- [MCP Server](#mcp-server)
- [Directory Structure](#directory-structure)
- [Architecture Areas](#architecture-areas)
- [SEO Topics and Search Terms](#seo-topics-and-search-terms)
- [Tech Stack](#tech-stack)
- [Usage Notes](#usage-notes)
- [Repository Health Files](#repository-health-files)
- [Disclaimer](#disclaimer)

---

## What is Claude Code?

Claude Code is Anthropic’s terminal-based coding assistant CLI. This repository focuses on a TypeScript source snapshot and presents it as a searchable archive for developers studying:

- CLI architecture
- tool systems
- command routing
- bridge systems
- permissions and policy handling
- terminal UI patterns with React + Ink
- MCP integration patterns

## Repository Highlights

| Area | What you get |
|---|---|
| **Source archive** | A large TypeScript CLI snapshot organized for inspection |
| **Documentation** | Architecture, commands, tools, subsystems, and exploration guides |
| **MCP server** | Interactive source exploration through Model Context Protocol tooling |
| **Public-facing structure** | Clear headings, searchable keywords, and descriptive metadata |
| **Maintainer branding** | Public-facing repo identity switched to Gary Doman / GareBear99 |

## Documentation

For in-depth guides, see the [`docs/`](docs/) directory:

| Guide | Description |
|-------|-------------|
| **[Architecture](docs/architecture.md)** | Core pipeline, startup sequence, state management, rendering, and data flow |
| **[Tools Reference](docs/tools.md)** | Catalog of agent tools, categories, and permission patterns |
| **[Commands Reference](docs/commands.md)** | Slash commands organized by category |
| **[Subsystems Guide](docs/subsystems.md)** | Deep dives into bridge systems, permissions, plugins, skills, tasks, and memory |
| **[Exploration Guide](docs/exploration-guide.md)** | Best entry points for navigating the codebase |
| **[Bridge Guide](docs/bridge.md)** | IDE bridge behavior and transport concepts |

Also see: [CONTRIBUTING.md](CONTRIBUTING.md) · [SECURITY.md](SECURITY.md) · [SUPPORT.md](SUPPORT.md) · [mcp-server/README.md](mcp-server/README.md)

## MCP Server

This repository includes an MCP server for interactive exploration of the source tree from MCP-compatible clients.

### Install from source

```bash
git clone https://github.com/GareBear99/claude-code-source-archive.git
cd claude-code-source-archive/mcp-server
npm install
npm run build
```

### Example registration

```bash
claude mcp add claude-code-source-explorer -- node /absolute/path/to/claude-code-source-archive/mcp-server/dist/index.js
```

### What the MCP server is for

- list tools
- inspect commands
- search source files
- read specific source paths
- browse subsystem layouts
- understand architecture faster than manual grepping


## Repository Health Files

This repository also includes standard GitHub/community files for a cleaner public release surface:

- [CHANGELOG.md](CHANGELOG.md)
- [RELEASE_CHECKLIST.md](RELEASE_CHECKLIST.md)
- [SECURITY.md](SECURITY.md)
- [SUPPORT.md](SUPPORT.md)
- [CODE_OF_CONDUCT.md](CODE_OF_CONDUCT.md)

## Directory Structure

```text
src/                 Core TypeScript source tree
commands/            Command implementations and routing
bridge/              IDE and remote bridge logic
cli/                 Terminal I/O, printing, transport, update logic
buddy/               Companion and notification related UI logic
docs/                Public-facing documentation and architecture notes
mcp-server/          Source exploration MCP server
prompts/             Prompt and reconstruction notes
scripts/             Build, test, and packaging scripts
```

## Architecture Areas

### 1. CLI runtime
Terminal entrypoints, output rendering, structured I/O, transports, and session flow.

### 2. Tool system
Tool definitions, invocation paths, permissions, and execution structure.

### 3. Command system
Slash commands, categories, handlers, and registry-level organization.

### 4. Bridge system
Remote sessions, trusted devices, polling, transport layers, and bridge UI/state.

### 5. MCP exploration layer
Source inspection tooling for faster research and developer onboarding.

## SEO Topics and Search Terms

This repository is intentionally structured to rank better for searches such as:

- Claude Code source code
- Claude Code source archive
- Claude Code TypeScript source
- Claude Code architecture
- Claude Code commands
- Claude Code tools
- Claude Code MCP server
- Claude Code reverse engineering
- Anthropic CLI source analysis
- React Ink terminal UI source
- Bun TypeScript CLI example
- Gary Doman Claude Code archive
- GareBear99 Claude Code research

## Tech Stack

| Topic | Stack |
|---|---|
| Language | TypeScript |
| Runtime | Bun |
| UI | React + Ink |
| MCP | Model Context Protocol |
| Packaging | npm-compatible Node tooling for MCP server |

## Usage Notes

This repo is best used as:

- a research archive
- a code-reading resource
- an architecture reference
- a public documentation surface for Claude Code source analysis

## Disclaimer

This repository is presented as an **unofficial archive and analysis resource** curated by Gary Doman. It is **not** an official Anthropic repository or product release.
