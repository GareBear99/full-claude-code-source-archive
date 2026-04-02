# Release Checklist

Use this before making the repository public or tagging a release.

## GitHub repository settings

- [ ] Repository name is `claude-code-source-archive`
- [ ] Description matches the README positioning
- [ ] Topics are added and match `docs/public-facing-seo.md`
- [ ] Social preview image is configured
- [ ] Discussions are enabled
- [ ] Issues and Projects are enabled if desired
- [ ] Default branch is correct

## Public-facing files

- [ ] `README.md` is accurate and links work
- [ ] `CONTRIBUTING.md`, `SECURITY.md`, `SUPPORT.md`, and `CODE_OF_CONDUCT.md` are present
- [ ] `LICENSE` and `NOTICE.md` still reflect the intended archive framing
- [ ] `CHANGELOG.md` is updated
- [ ] `RELEASE_SURFACE_AUDIT.md` still reflects the current state

## Package / MCP metadata

- [ ] root `package.json` metadata is correct
- [ ] `web/package.json` metadata is correct
- [ ] `server.json` and `mcp-server/server.json` match the GitHub repo and package identifiers
- [ ] npm package names and versions are intentional

## Workflows

- [ ] CI workflow reflects the behavior you actually want
- [ ] publish workflow uses the correct npm token and registry metadata
- [ ] tag naming and versioning are consistent

## Content audit

- [ ] No stale links to prior repo owners remain in public-facing docs
- [ ] No accidental secrets or credentials are present
- [ ] README language does not overstate official status
