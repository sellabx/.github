# Maintainers Guide

This guide defines operational responsibilities for maintainers of sellabx organization governance and repository standards.

## Roles

- Maintainer: reviews and merges contributions, triages issues, and enforces standards.
- Security contact: coordinates private vulnerability handling.
- Release owner: prepares release notes, tags, and rollback checks.

## Daily Responsibilities

- Triage new issues and pull requests.
- Apply/adjust labels and priority.
- Ensure templates are used correctly.
- Keep discussions respectful and aligned with `CODE_OF_CONDUCT.md`.

## Issue and PR SLA Targets

- New issue triage: within 2 business days.
- First PR review response: within 2 business days.
- Security report acknowledgement: within 72 hours.

## Incident and Escalation

Escalate immediately when any of the following occurs:

- Security risk with active exploit potential
- Production-impacting regression
- Data integrity or privacy risk

Escalation path:

1. Notify security contact or incident owner.
2. Create a private tracking thread if needed.
3. Assign an accountable maintainer.
4. Track mitigation, rollback, and follow-up tasks.

## Release Window and Freeze Guidance

- Prefer releases during agreed low-risk windows.
- Use temporary freeze during active incidents or high-risk migrations.
- Do not merge high-risk changes without clear rollback notes.

## Review Quality Bar

Before merge, verify:

- Conventional Commit compliant title
- Relevant tests and lint checks passed
- Risk and rollback notes present for risky changes
- Documentation updates included where needed
- No secrets or sensitive data in diff

## Post-Incident Follow-up

For high-impact incidents:

- Create a public or internal postmortem summary as appropriate.
- Record root cause, contributing factors, and corrective actions.
- Track preventive actions to completion.
