# Contributing

Thanks for your interest in contributing to this repository.

## What This Repository Is

This repository is an **unofficial archive, documentation hub, and exploration toolkit** maintained by **Gary Doman / GareBear99**. The focus is public-facing developer readability, architecture notes, MCP tooling, and repository discoverability.

## Good Contribution Targets

- **Documentation** — improve `docs/`, diagrams, onboarding, and architecture write-ups
- **Repository polish** — metadata, badges, issue templates, release notes, and discoverability improvements
- **MCP tooling** — improvements inside `mcp-server/`
- **Analysis** — command references, subsystem notes, and codebase walkthroughs
- **Supporting scripts** — tooling that helps inspect, index, or explore the snapshot

## What To Avoid Changing By Default

- **`src/`** — treat the archived snapshot as a reference baseline unless a maintainer explicitly approves changes
- **Historical framing** — do not rewrite the archive into an “official release” claim

## Local Setup

```bash
git clone https://github.com/GareBear99/claude-code-source-archive.git
cd claude-code-source-archive
```

### MCP Server

```bash
cd mcp-server
npm install
npm run dev
npm run build
```

### Root checks

```bash
npm run lint
npm run typecheck
```

## Style

For new code and docs:

- TypeScript where applicable
- Clear naming
- Minimal, useful comments
- Keep public-facing copy consistent with Gary Doman / GareBear99 branding

## Pull Requests

1. Fork the repo
2. Create a branch
3. Keep changes scoped
4. Open a pull request with a clear summary

Please keep pull requests focused on archive quality, documentation quality, MCP tooling, or safe repository improvements unless a maintainer explicitly asks for deeper source changes.

## Maintainer

Open an issue in the repository for questions, fixes, or release-surface improvements.
