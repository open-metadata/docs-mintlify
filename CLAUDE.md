# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Development Commands

- `npm run dev` - Start the Mintlify development server for local documentation preview
- No test command is currently configured (package.json shows placeholder test script)

## Project Overview

This is a documentation site for **Collate**, a unified platform for data discovery, lineage, and governance. The project uses **Mintlify** as the documentation framework.

### Architecture

- **Framework**: Mintlify documentation platform
- **Content Format**: MDX files for documentation pages
- **Configuration**: `docs.json` contains the complete site structure and navigation
- **Dependencies**: React 19.1.1 and Mint 4.2.108

### Content Organization

The documentation is organized into main tabs:
- **Home**: Landing page (`index.mdx`)
- **Administration**: User management, roles, customization, maintenance
- **Guides**: Feature-specific documentation organized by user roles and capabilities
  - Users: Basic operations, discovery, collaboration
  - Data Quality: Profiler, tests, incident management, observability
  - Data Governance: Classification, glossary, domains, workflows
  - Data Lineage: Exploration and management
  - Data Insights: Analytics and reporting
- **Integrations**: MCP (Model Context Protocol) integrations

### Key Configuration Files

- `docs.json`: Complete site navigation structure, theme configuration, and page organization
- `package.json`: Project dependencies and development scripts
- `index.mdx`: Homepage content with feature overview cards

### Content Structure Patterns

- Each section follows a consistent pattern with overview pages and detailed guides
- Pages use MDX format with frontmatter for title and description
- Card components are used extensively for navigation and feature highlighting
- Hierarchical organization with groups and subgroups in navigation

### Working with Documentation

- All content files are `.mdx` format supporting React components
- Navigation structure is defined centrally in `docs.json`
- Theme uses "palm" template with custom branding colors (#cd3c4d)
- Images and assets are stored in `/images/` directory