# Git Structure and Contribution Guidelines

---

## Branch Strategy

Branches should follow a clear naming convention to make development and code reviews easier.

### Branch Types

|Branch|Purpose|
|---|---|
|`feature/<task-name>`|New features and enhancements|
|`bugfix/<issue-name>`|Bug fixes and issue resolution|
|`docs/<document-name>`|Documentation updates|
|`chore/<task-name>`|Maintenance tasks, dependency updates, CI/CD changes, configuration updates|
|`refactor/<task-name>`|Code refactoring and performance improvements|

### Examples

```text
feature/user-authentication
feature/url-expiration

bugfix/invalid-token
bugfix/duplicate-shortcode

docs/api-authentication
docs/deployment-guide

chore/update-dependencies
chore/github-actions

refactor/url-generation-service
refactor/database-query-optimization
```

---

## Commit Convention

Commits should follow a consistent format to improve readability and maintain a clean project history.

### Commit Types

|Type|Description|
|---|---|
|`feat:`|New feature or enhancement|
|`fix:`|Bug fix|
|`docs:`|Documentation changes|
|`chore:`|Maintenance and non-functional changes|
|`refactor:`|Code refactoring without changing behavior|

### Commit Format

```text
<type>: <short description>
```

### Examples

```text
feat: implement email-based authentication

fix: resolve duplicate shortcode generation

docs: update API authentication guide

chore: update project dependencies

refactor: optimize URL lookup queries
```

---

## Commit Description

When additional context is needed, provide a detailed commit body.

### Example

```bash
git commit \
    -m "feat: implement email-based authentication" \
    -m "- Add email login support." \
    -m "- Update authentication backend." \
    -m "- Add validation tests for authentication flow."
```

### Guidelines

- Use the first line as a concise summary.
    
- Keep the summary focused on the purpose of the change.
    
- Use additional message blocks when more details are required.
    
- Describe what changed and why it was necessary.
    

---

## Issues

Issues represent tasks, improvements, bugs, and discussions related to the project.

### Rules

- Create an issue before starting significant work.
    
- Use the appropriate issue template whenever available.
    
- Provide a clear description of the problem or enhancement.
    
- Include reproduction steps for bugs.
    
- Add the `in-progress` label when actively working on an issue.
    
- Keep issue discussions relevant and constructive.
    

### Recommendations

- Link related issues whenever possible.
    
- Ask questions directly within the issue discussion.
    
- Propose solutions before implementing major architectural changes.
    

---

## Pull Requests

All code changes should be submitted through a Pull Request (PR).

### Requirements

- Follow the Pull Request template.
    
- Provide a clear description of the changes.
    
- Link all related issues.
    
- Add appropriate labels.
    
- Assign yourself if applicable.
    
- Request at least one reviewer.
    

### Review Process

- Do not merge your own Pull Request unless explicitly authorized by the maintainers.
    
- Address review comments before requesting another review.
    
- Ensure all checks and tests pass before merging.
    
- Keep Pull Requests focused on a single purpose whenever possible.
    

### Pull Request Checklist

-  Branch follows the naming convention
    
-  Commits follow the commit convention
    
-  Related issue is linked
    
-  Documentation updated if necessary
    
-  Tests added or updated if necessary
    
-  CI checks are passing
    
-  Reviewer assigned
    

---

## General Guidelines

- Keep changes small and focused.
    
- Write meaningful commit messages.
    
- Prefer multiple small Pull Requests over large ones.
    
- Update documentation whenever behavior changes.
    
- Maintain backward compatibility whenever possible.
    
- Respect code review feedback and team decisions.
    

---

> Consistency is more important than perfection. Following the same workflow across the project makes collaboration easier, improves maintainability, and keeps the repository organized as it grows.

---

**Author:** Richie Pagard  
**Topic:** Git Structure for Pijamas Team  
**Created:** June 03, 2026

