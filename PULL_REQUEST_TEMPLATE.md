# Pull Request

## Conventional Commits Compliance

PR title must follow Conventional Commits:

`<type>(<optional-scope>): <summary>`

Examples:

- `feat(api): add tenant-aware throttling`
- `fix(ci): restore cache fallback behavior`

## 1. Change Description

Describe what changed and why.

## 2. Related Issues

Link related issues using keywords, for example:

- `closes #123`
- `refs #456`

## 3. Testing Performed

Describe test coverage and results.

- Unit tests:
- Integration tests:
- Manual verification:

## 4. Type of Change

- [ ] Bug fix
- [ ] Feature
- [ ] Enhancement
- [ ] Documentation

## 5. Checklist

- [ ] PR title follows Conventional Commits
- [ ] Code is linted and formatting checks pass
- [ ] Unit tests added or updated where needed
- [ ] Relevant tests pass locally
- [ ] Documentation updated where needed
- [ ] No secrets or credentials committed
- [ ] Backward compatibility reviewed
- [ ] Rollback considerations documented for risky changes

## Review Notes

Provide context that helps reviewers assess risk, architecture impact, and rollout safety.
