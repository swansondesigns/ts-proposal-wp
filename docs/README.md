# WordPress Development Proposal Site

A Docsify-powered static site for presenting WordPress development proposals. The site features a professional design with custom typography and is deployed via GitHub Pages.

## Development Guidelines

### Commit Standards

This project follows strict commit practices to maintain code quality and project history:

#### Commit Message Format

All commit messages **must** follow the [Conventional Commits](https://www.conventionalcommits.org/) specification:

```
<type>[optional scope]: <description>

[optional body]

[optional footer(s)]
```

**Examples:**

```
feat: add dark mode toggle functionality
fix(styles): correct sidebar alignment in mobile view
docs: update development guidelines
style: format CSS variables for better readability
refactor: reorganize dark mode variables
```

#### Commit Types

-   **feat:** A new feature
-   **fix:** A bug fix
-   **docs:** Documentation only changes
-   **style:** Changes that do not affect the meaning of the code (white-space, formatting, etc.)
-   **refactor:** A code change that neither fixes a bug nor adds a feature
-   **test:** Adding missing tests or correcting existing tests
-   **chore:** Changes to the build process or auxiliary tools

### Workflow Requirements

#### Human-Initiated Commits

-   **All commits are user-initiated** - No automated commits without explicit human approval
-   **Commit messages must be presented to the user** before execution for review and approval
-   Users have final authority over all commit messages and timing

#### Pre-Commit Checklist

Before any commit, ensure:

-   [ ] Commit message follows conventional format
-   [ ] Commit message accurately describes the changes
