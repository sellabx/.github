# Release and Change Management

This repository follows a predictable, low-risk release model suitable for scalable business infrastructure.

## Versioning

- Use Semantic Versioning (`MAJOR.MINOR.PATCH`).
- `PATCH`: backward-compatible fixes.
- `MINOR`: backward-compatible features.
- `MAJOR`: breaking changes.

## Release Cadence

- Regular releases: weekly or bi-weekly, depending on merged changes.
- Critical fixes: out-of-band hotfix releases.
- Security fixes: prioritized and released as soon as validated.

## Release Branch and Tag Strategy

- Default integration branch: `main`.
- Release source: latest stable commit on `main`.
- Tags must follow `vX.Y.Z` format.
- Every release tag must map to a changelog entry.

## Change Entry Requirements

Every merged PR should include:

- Change summary (what and why)
- Risk level and rollback notes (when relevant)
- Test evidence
- Issue linkage (`closes #123` or `refs #123`)

## Changelog Policy

- Maintain changelog in `CHANGELOG.md`.
- Group entries by release version and date.
- Categorize entries: `Added`, `Changed`, `Fixed`, `Security`.
- Keep user-impacting and operationally relevant details concise and actionable.

## Pre-Release Checklist

- Required CI checks pass
- Relevant tests pass
- No known blocker issues
- Changelog updated
- Rollback path confirmed for risky changes

## Rollback

- Rollback mechanism: revert offending commits or redeploy previous stable release tag.
- For incidents, open a follow-up issue with root cause and preventive actions.

## Communication

- Publish release notes for each tagged release.
- Clearly call out breaking changes, migration requirements, and security updates.
