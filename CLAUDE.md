# CLAUDE.md - AI Assistant Guide

> **Last Updated**: 2025-12-02
> **Repository**: jansherkhan3/jansherkhan3
> **Status**: Empty/Initial Setup

## Table of Contents

1. [Repository Overview](#repository-overview)
2. [Codebase Structure](#codebase-structure)
3. [Development Workflows](#development-workflows)
4. [Key Conventions](#key-conventions)
5. [Git Workflow](#git-workflow)
6. [Testing Guidelines](#testing-guidelines)
7. [AI Assistant Guidelines](#ai-assistant-guidelines)
8. [Common Tasks](#common-tasks)

---

## Repository Overview

### Current State
This repository is currently in its initial setup phase with no project files or code yet committed. This document serves as a living guide that will be updated as the project develops.

### Purpose
*To be defined as the project develops*

### Technology Stack
*To be defined*

### Key Dependencies
*To be defined*

---

## Codebase Structure

### Current Directory Layout
```
jansherkhan3/
├── .git/              # Git repository data
└── CLAUDE.md          # This file
```

### Planned Structure
*This section should be updated once the project structure is established*

```
jansherkhan3/
├── .git/              # Git repository data
├── .gitignore         # Git ignore patterns
├── README.md          # Project documentation
├── CLAUDE.md          # AI assistant guide (this file)
├── src/               # Source code (TBD based on project type)
├── tests/             # Test files
├── docs/              # Additional documentation
└── [config files]     # Project-specific configuration
```

### Key Directories (Template)
- **`src/`** or **`lib/`**: Main source code
- **`tests/`** or **`__tests__/`**: Test files
- **`docs/`**: Documentation files
- **`scripts/`**: Build, deployment, or utility scripts
- **`config/`**: Configuration files

---

## Development Workflows

### Initial Setup
1. **Clone the repository**:
   ```bash
   git clone http://127.0.0.1:18634/git/jansherkhan3/jansherkhan3
   cd jansherkhan3
   ```

2. **Install dependencies** (once defined):
   ```bash
   # Example for Node.js:
   npm install

   # Example for Python:
   pip install -r requirements.txt

   # Example for Go:
   go mod download
   ```

3. **Set up development environment**:
   *To be defined based on project requirements*

### Standard Development Cycle
1. **Create a feature branch**:
   ```bash
   git checkout -b feature/your-feature-name
   ```

2. **Make changes and test locally**

3. **Commit with descriptive messages**:
   ```bash
   git add .
   git commit -m "type: clear description of changes"
   ```

4. **Push changes**:
   ```bash
   git push -u origin feature/your-feature-name
   ```

5. **Create pull request** (if applicable)

---

## Key Conventions

### Code Style
*To be defined based on project language and team preferences*

**General Principles**:
- Write clear, self-documenting code
- Use consistent naming conventions
- Keep functions small and focused
- Comment complex logic, not obvious code
- Follow language-specific best practices

### Commit Message Format
Use conventional commits format:
```
<type>: <description>

[optional body]

[optional footer]
```

**Types**:
- `feat`: New feature
- `fix`: Bug fix
- `docs`: Documentation changes
- `style`: Code style changes (formatting, etc.)
- `refactor`: Code refactoring
- `test`: Adding or updating tests
- `chore`: Maintenance tasks
- `perf`: Performance improvements

**Examples**:
```
feat: add user authentication module
fix: resolve memory leak in data processor
docs: update API documentation
refactor: simplify error handling logic
```

### Naming Conventions
*To be defined based on project language*

**General Guidelines**:
- Use descriptive, meaningful names
- Avoid abbreviations unless widely understood
- Be consistent with casing conventions (camelCase, snake_case, PascalCase)
- Use verbs for functions/methods
- Use nouns for variables/classes

---

## Git Workflow

### Branch Strategy

**Current Working Branch**: `claude/claude-md-miouv44ubkggehq8-01EU3bMFiSVkXNsRmLRUjWvg`

**Branch Naming Conventions**:
- `main` or `master`: Production-ready code
- `develop`: Integration branch for features
- `feature/*`: New features (e.g., `feature/user-auth`)
- `fix/*`: Bug fixes (e.g., `fix/login-error`)
- `hotfix/*`: Urgent production fixes
- `claude/*`: AI assistant working branches

### Git Configuration

**Remote**:
```
URL: http://local_proxy@127.0.0.1:18634/git/jansherkhan3/jansherkhan3
```

**Important Git Operations**:

**Push with retry logic** (for network reliability):
```bash
# Always use -u flag for new branches
git push -u origin <branch-name>

# For claude/* branches, ensure session ID matches
```

**Fetch specific branches**:
```bash
git fetch origin <branch-name>
```

**Pull with branch specification**:
```bash
git pull origin <branch-name>
```

### Merge Strategy
*To be defined (e.g., merge commits, squash, rebase)*

---

## Testing Guidelines

### Test Structure
*To be defined based on project testing framework*

### Running Tests
*To be defined*

```bash
# Example commands:
# npm test
# pytest
# go test ./...
```

### Test Coverage
*Set coverage goals when project is established*

### Writing Tests
**Best Practices**:
- Write tests for new features
- Test edge cases and error conditions
- Keep tests isolated and independent
- Use descriptive test names
- Mock external dependencies

---

## AI Assistant Guidelines

### General Principles for AI Assistants

1. **Always Read Before Modifying**
   - Never propose changes to code you haven't read
   - Use Read tool before Edit tool
   - Understand context before suggesting modifications

2. **Minimize Over-Engineering**
   - Only make changes that are directly requested or clearly necessary
   - Keep solutions simple and focused
   - Don't add features beyond what was asked
   - Don't add unnecessary error handling, abstractions, or future-proofing

3. **Code Quality**
   - Write secure code (avoid XSS, SQL injection, command injection, etc.)
   - Follow existing code patterns in the repository
   - Maintain consistency with the codebase style
   - Don't add comments or docstrings to unchanged code

4. **Task Management**
   - Use TodoWrite tool for complex multi-step tasks
   - Break down large tasks into manageable steps
   - Mark tasks as completed immediately after finishing
   - Keep user informed of progress

5. **Git Operations**
   - Always develop on the designated branch
   - Commit with clear, descriptive messages
   - Never skip hooks or use force push without permission
   - Push to origin when changes are complete

6. **Communication**
   - Be concise and direct
   - Avoid unnecessary emojis
   - Focus on technical accuracy
   - Provide objective guidance

### Workflow for AI Assistants

#### For Questions/Analysis:
1. Use Task tool with subagent_type=Explore for broad codebase questions
2. Use Glob/Grep for specific file or keyword searches
3. Read relevant files
4. Provide detailed, accurate answers with file references

#### For Implementation Tasks:
1. **Plan**: Use TodoWrite to create task list
2. **Explore**: Read relevant existing code
3. **Implement**: Make changes using Edit/Write tools
4. **Verify**: Check that changes work as intended
5. **Commit**: Commit changes with descriptive message
6. **Push**: Push to the designated branch

### File References

When referencing code, always use the format:
```
file_path:line_number
```

Example: "The error handling is in src/utils/api.js:142"

### Working with This Repository

**Current Branch**: `claude/claude-md-miouv44ubkggehq8-01EU3bMFiSVkXNsRmLRUjWvg`

**Push Protocol**:
- Branch must start with `claude/` and end with matching session ID
- Use `git push -u origin <branch-name>`
- Retry up to 4 times with exponential backoff (2s, 4s, 8s, 16s) on network errors

**Fetch/Pull Protocol**:
- Prefer fetching specific branches
- Retry up to 4 times with exponential backoff on network failures

---

## Common Tasks

### Adding New Features
1. Read existing code to understand current patterns
2. Plan implementation using TodoWrite
3. Write code following existing conventions
4. Add tests for new functionality
5. Update documentation if needed
6. Commit and push changes

### Fixing Bugs
1. Reproduce the bug if possible
2. Identify root cause by reading relevant code
3. Implement minimal fix
4. Verify fix works
5. Add test to prevent regression
6. Commit with clear bug description

### Refactoring
1. Only refactor when explicitly requested
2. Ensure tests pass before and after
3. Make incremental changes
4. Don't change behavior, only structure
5. Commit refactoring separately from features

### Documentation Updates
1. Keep documentation in sync with code
2. Update this file (CLAUDE.md) when conventions change
3. Use clear, concise language
4. Include examples where helpful

---

## Project-Specific Notes

### Important Gotchas
*To be added as discovered*

### Performance Considerations
*To be added as relevant*

### Security Considerations
*To be added based on project requirements*

### Known Issues
*Track known issues or limitations*

---

## Updating This Document

This document should be updated whenever:
- Project structure changes significantly
- New conventions are established
- Development workflows change
- Important patterns or gotchas are discovered
- New tooling or dependencies are added

**Maintenance**: All developers and AI assistants should keep this document current to ensure it remains a reliable guide for working with the codebase.

---

## Additional Resources

### Documentation
- README.md (to be created)
- API documentation (if applicable)
- Architecture diagrams (if applicable)

### External Links
*Add links to relevant external documentation, style guides, framework docs, etc.*

---

**Note**: This is a living document. As the project evolves, update this file to reflect the current state of the repository, development practices, and team conventions.
