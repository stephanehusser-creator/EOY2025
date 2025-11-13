# CLAUDE.md - AI Assistant Guide

This document provides comprehensive guidance for AI assistants working with the EOY2025 presentation repository.

## Repository Overview

**Purpose**: This repository contains documentation and resources for the End of Year 2025 presentation project.

**Type**: Documentation-focused repository with Markdown files and reference materials.

**Current State**: Early development phase with foundational documentation structure in place.

## Repository Structure

```
EOY2025/
├── CLAUDE.md              # This file - AI assistant guidance
├── README.md              # Project overview and entry point
└── docs/                  # Main documentation directory
    ├── README.md          # Documentation overview
    ├── getting-started.md # Setup and onboarding guide
    ├── presentation-notes.md # Presentation outline and content
    └── sources/           # Reference materials and sources
        └── README.md      # Source organization guide
```

## Key Conventions

### Documentation Standards

1. **Markdown Format**: All documentation uses GitHub-flavored Markdown
2. **File Organization**:
   - Keep documentation in the `docs/` directory
   - Use clear, descriptive filenames in kebab-case
   - Maintain a flat structure unless complexity requires subdirectories

3. **Content Structure**:
   - Start each document with a level-1 heading (`#`)
   - Use hierarchical headings (H1 → H2 → H3)
   - Include a brief introduction/overview section
   - Add code blocks with language specifiers for examples
   - Use bullet points and numbered lists for clarity

4. **File Naming**:
   - General docs: `descriptive-name.md`
   - Source materials: `YYYY-MM-DD-descriptive-name.ext`
   - Example: `2025-01-15-market-research-data.pdf`

### Git Workflow

1. **Branch Naming**:
   - Feature branches: `claude/claude-md-{identifier}`
   - Always work on feature branches, never directly on main
   - Branch names should be descriptive of the work being done

2. **Commit Messages**:
   - Use clear, descriptive commit messages
   - Start with a verb in present tense (Add, Update, Fix, Remove)
   - Reference the type of change (documentation, structure, content)
   - Examples:
     - "Add sources folder under docs for reference materials"
     - "Update getting-started guide with dependency instructions"

3. **Commit Workflow**:
   - Stage relevant files with `git add`
   - Commit with descriptive messages
   - Push to feature branch with `git push -u origin <branch-name>`
   - Use exponential backoff retry (2s, 4s, 8s, 16s) for network errors

## Development Workflows

### Adding New Documentation

1. **Determine Location**:
   - General documentation → `docs/`
   - Reference materials → `docs/sources/`
   - Root-level only for project-wide files (README, LICENSE, etc.)

2. **Create Content**:
   - Follow markdown standards
   - Include clear headings and structure
   - Add examples where helpful
   - Link to related documents

3. **Update Index**:
   - Update `docs/README.md` structure section
   - Add links in root `README.md` if appropriate
   - Ensure navigation is intuitive

4. **Commit Changes**:
   - Stage new files
   - Write descriptive commit message
   - Push to feature branch

### Updating Existing Documentation

1. **Read Current Content**: Always read the file before editing
2. **Make Focused Changes**: Edit specific sections without unnecessary rewrites
3. **Maintain Style**: Keep consistent with existing formatting and tone
4. **Update Related Docs**: Check if other documents need updates for consistency
5. **Commit Clearly**: Explain what was updated and why

### Adding Reference Materials

1. **Location**: Place in `docs/sources/`
2. **Naming**: Use date-based naming `YYYY-MM-DD-descriptive-name.ext`
3. **Organization**: Create subdirectories by topic if needed
4. **Attribution**: Include source information and attribution
5. **Documentation**: Update `docs/sources/README.md` if adding new categories

## File-Specific Guidance

### README.md (Root)
- **Purpose**: Project overview and entry point for new users
- **Content**: High-level introduction, structure overview, navigation links
- **Update When**: Major structural changes, new sections added, project scope changes

### docs/README.md
- **Purpose**: Documentation hub and navigation
- **Content**: Overview of all documentation, structure guide, contribution guidelines
- **Update When**: New documentation files added, reorganization occurs

### docs/getting-started.md
- **Purpose**: Onboarding guide for new contributors
- **Content**: Prerequisites, setup instructions, first steps
- **Update When**: Dependencies change, setup process updates, new tools added

### docs/presentation-notes.md
- **Purpose**: Core presentation content and structure
- **Content**: Outline, key messages, objectives, resources
- **Update When**: Presentation content evolves, structure changes

### docs/sources/README.md
- **Purpose**: Guide for organizing reference materials
- **Content**: Organization system, naming conventions, guidelines
- **Update When**: New source categories added, organization system changes

## Best Practices for AI Assistants

### Understanding Context

1. **Repository Stage**: This is an early-stage documentation project
2. **Flexibility**: Many sections have placeholders - fill them when appropriate
3. **Documentation Focus**: No source code currently - this is pure documentation
4. **Presentation Goal**: All content supports the EOY2025 presentation

### Making Changes

1. **Read First**: Always read existing files before editing
2. **Preserve Structure**: Maintain established organization patterns
3. **Be Consistent**: Match existing style, tone, and formatting
4. **Link Documents**: Ensure cross-references stay valid
5. **Think Holistically**: Consider impact on related documents

### Communication

1. **Be Concise**: Clear, direct explanations
2. **Show Structure**: Use code blocks to show file organization
3. **Reference Locations**: Use `path/to/file.md:line_number` format
4. **Explain Decisions**: When making choices, briefly explain reasoning

### Git Operations

1. **Branch Awareness**: Always work on the designated feature branch
2. **Commit Frequency**: Commit logical units of work
3. **Push Protocol**: Use `git push -u origin <branch-name>` with retry logic
4. **Clean History**: Each commit should represent a complete, logical change

## Common Tasks Reference

### Create New Documentation File

```bash
# 1. Create the file in appropriate location
# 2. Add content following markdown standards
# 3. Update relevant index files
# 4. Commit and push
git add docs/new-file.md
git add docs/README.md  # if updated
git commit -m "Add documentation for [topic]"
git push -u origin <branch-name>
```

### Update Repository Structure

1. Create new directories/files as needed
2. Update all README files that reference structure
3. Update navigation links in affected documents
4. Update this CLAUDE.md if workflow changes
5. Commit all changes together

### Add Reference Materials

```bash
# 1. Place file in docs/sources/ with proper naming
# 2. Create subdirectory if starting a new category
# 3. Update docs/sources/README.md if needed
git add docs/sources/
git commit -m "Add reference material: [description]"
git push -u origin <branch-name>
```

## Questions to Consider

When working on this repository, ask yourself:

1. **Structure**: Does this change maintain clear organization?
2. **Navigation**: Can users easily find this information?
3. **Consistency**: Does this match existing patterns?
4. **Completeness**: Are related documents updated too?
5. **Clarity**: Will this be clear to someone new to the project?

## Project Evolution

This repository is in early stages. Expect:

- Content to be added to placeholder sections
- Structure to evolve as needs are clarified
- New documentation files as topics emerge
- Reference materials to accumulate in `docs/sources/`

When adding substantial new content or structure, consider updating this CLAUDE.md to reflect new conventions or workflows.

## Getting Help

- Review existing documentation structure for patterns
- Check git history for examples: `git log --oneline`
- Read related documents for context
- When uncertain, preserve existing style and ask for clarification

---

**Last Updated**: 2025-11-13
**Repository Stage**: Early Development
**Primary Focus**: Documentation Structure & Presentation Content
