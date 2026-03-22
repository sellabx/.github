# Contributing to sellabx

Thank you for contributing to sellabx.
We build scalable tools and infrastructure for business-critical workloads across industries.

## Contribution Workflow

### 1. Fork

Fork the repository to your own GitHub account.

### 2. Branch

Create a branch from `main` with a descriptive name.

- `feat/<short-description>`
- `fix/<short-description>`
- `chore/<short-description>`
- `docs/<short-description>`
- `refactor/<short-description>`

### 3. Build Your Change

- Keep changes focused and minimal.
- Follow existing architecture and naming patterns.
- Add or update documentation when behavior changes.

### 4. Commit Using Conventional Commits

Commit messages must follow this format:

`<type>(<optional-scope>): <short summary>`

Supported types:

- `feat`
- `fix`
- `docs`
- `refactor`
- `test`
- `chore`
- `ci`
- `perf`

Examples:

- `feat(api): add tenant-aware rate limiting`
- `fix(worker): prevent duplicate retry scheduling`
- `ci(github): cache dependency installation`

For breaking changes, use `!` and explain in the commit body:

- `feat(auth)!: replace legacy token contract`

### 5. Validate Locally

Before opening a PR:

1. Run linting.
2. Run unit tests.
3. Run any integration tests relevant to your change.
4. Confirm no secrets or credentials are committed.

### 6. Open a Pull Request

Open a PR against `main` and complete the PR template.

- Use a PR title that follows Conventional Commits.
- Link related issues, for example `closes #123`.
- Include testing evidence and rollout notes for operational changes.

### 7. Review and Merge

- Respond to review comments clearly and promptly.
- Keep your branch up to date with `main`.
- A maintainer merges after approvals and required checks pass.

## Coding Standards

- Write clear, maintainable, production-ready code.
- Prefer readability over clever implementations.
- Add deterministic tests for critical paths.
- Ensure lint checks pass before requesting review.
- Avoid unrelated refactors in the same PR.
- Include logging and metrics hooks where operational visibility matters.

## Issue Triage Process

All incoming issues are triaged by maintainers.

1. **Validate**: confirm the report has enough context and reproduction details.
2. **Classify**: mark as bug, feature, question, or documentation.
3. **Prioritize**: assess business and operational impact.
4. **Route**: assign an owner or place in backlog.
5. **Track**: update labels and status, then communicate next steps.

Priority guidance:

- High: production outages, data risk, security, critical reliability regressions
- Medium: significant functional problems with workaround
- Low: minor defects, UX polish, or non-blocking enhancements

## Reporting Security Issues

Do not open public issues for security vulnerabilities.
Follow the process in [SECURITY.md](SECURITY.md).

## Community and Conduct

By participating, you agree to follow [CODE_OF_CONDUCT.md](CODE_OF_CONDUCT.md).
