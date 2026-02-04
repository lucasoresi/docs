# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

OptaCost documentation site built with **Mintlify**. This is a documentation-only repository - no application code, builds, or tests. All content is in Spanish.

## Documentation Platform

- **Framework**: Mintlify (automatic builds and deployments on git push)
- **Format**: MDX (Markdown with React components)
- **Configuration**: `mint.json` (navigation, theming, tabs, social links)

## Key MDX Components Available

- `CardGroup`, `Card` - Feature cards and grids
- `Accordion`, `AccordionGroup` - Collapsible content
- `Steps`, `Step` - Step-by-step guides
- `Note`, `Info`, `Warning`, `Tip` - Callout boxes
- `CodeGroup` - Multi-language code examples
- `Tabs`, `Tab` - Tabbed content

## Content Structure

```
/                        # Root
├── mint.json            # Mintlify config (navigation, theme, tabs)
├── introduction.mdx     # Landing page
├── introduccion/        # Getting started (3 docs)
├── caracteristicas/     # Feature guides (8 docs)
├── api-reference/       # REST API documentation (12+ endpoint docs)
├── arquitectura/        # Technical architecture (4 docs)
└── guias/               # How-to guides (5 docs)
```

## MDX Frontmatter Format

Every documentation page requires:
```yaml
---
title: "Page Title"
description: "Brief description for SEO"
icon: "icon-name"  # Font Awesome icon (optional)
---
```

## Adding New Pages

1. Create `.mdx` file in appropriate directory
2. Add frontmatter with title, description, and optional icon
3. Add page path to `mint.json` navigation array under correct group
4. Commit - Mintlify auto-deploys

## Navigation Configuration

Edit `mint.json` to modify:
- `navigation` - Sidebar structure and page ordering
- `tabs` - Top-level navigation tabs
- `topbarLinks` / `topbarCtaButton` - Header buttons
- `colors` - Theme colors
- `anchors` - Quick-access links
