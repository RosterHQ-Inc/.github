# Roster HQ

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository Overview

This is the **Roster HQ `.github` organization repository** — a special GitHub repository that configures organization-wide settings and displays the public organization profile.

**This repository is PUBLIC.** GitHub requires this for the org profile README to display.

**Purpose**:
- Display organization profile README on https://github.com/RosterHQ-Inc
- Store organization-wide GitHub configuration templates (issues, PRs, discussions)
- Define default community health files for all organization repositories

## Repository Structure

```
.github/
├── .github/
│   └── PULL_REQUEST_TEMPLATE.md      # Default PR template for all org repos
├── profile/
│   └── README.md                     # Organization profile page (PUBLIC)
├── assets/
│   └── icons/
│       ├── rosterhq.png              # Organization logo PNG
│       └── rosterhq.svg              # Organization logo SVG
├── .gitignore
└── CLAUDE.md                         # This file
```

> **Note**: `.github/docs/` and `.claude/` are gitignored (agent local files)

## Important Gotchas

1. **Immediate Visibility**: Changes to `profile/README.md` appear immediately on https://github.com/RosterHQ-Inc when pushed to `main`. Review carefully before pushing.

2. **Organization-Wide Impact**: Templates and community health files in this repo become defaults for ALL Roster HQ repositories. Test thoroughly.

3. **Repository Overrides**: Individual repositories can override these defaults by creating their own `.github/` files. Organization templates are fallbacks.

5. **Public Information Only**: This repository is PUBLIC. Never include:
   - API keys, tokens, passwords
   - Internal infrastructure details
   - Customer information
   - Non-public product features
   - Proprietary CI tooling

## Development Standards

### Template Standards

**Pull Request Templates**:
- Enforce Linear issue reference (AAA-#### format)
- Checklist for tests, docs, breaking changes
- Imperative mood in title

**Community Files**:
- Clear, actionable guidance
- Professional and welcoming tone

## Git Workflow

### Commit Message Format

Use imperative mood. If no Linear issue, use descriptive summary only.

### Branching Strategy

- Main branch: `main`
- Feature branches: `user/description` or `user/linear-id-description`
- Always create PR for profile changes (require review)

## Key Files

- `profile/README.md` - Organization profile page (PUBLIC, visible on github.com/RosterHQ-Inc)
- `.github/PULL_REQUEST_TEMPLATE.md` - Default PR template for all org repos
